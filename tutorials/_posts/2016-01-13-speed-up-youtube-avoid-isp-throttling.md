---
title: 'Speed up youtube &#038; avoid time warner ISP throttling'
image: /assets/2016/02/twc.jpg
---
## ISP throttling

Time Warner Cable (TWC) and a few other internet providers can do a sneaky thing (probably stated in their terms of service somewhere) where they throttle your internet download speed when streaming (and uploading) a youtube (or similar stream based sites such as Netflix, Hulu, Twitch, etc.) video.

I have the basic Time Warner Cable package that includes phone, cable and internet. Using speedtest.net, I normally had anywhere from 1-10 mb/s download, and always under 1mb/s upload (when I was paying for 15mb/s). This is because Time Warner Cable was throttling the internet.

> Note: some speed test websites can show inaccurate results. Try using a couple unaffiliated speed testing sites.

## Use Google's public DNS

A quick tip for speeding up **all** websites, even if only a little is by changing from your current, default DNS to Google's. A DNS is essentially a phone book for the internet. When you go to a website, your computer (or router) performs a DNS lookup before it downloads it. Routers will often default to use your internet service provider's DNS. To change your router's DNS to Google's public DNS for faster and more secure DNS lookups:

Go to your router's home page (common one is [192.168.1.1](http://192.168.1.1/)) and navigate to the internet section. On this page, you should find a _Domain Name Server (DNS) Address_ header. Remove any default values (or change it to _Use These DNS Servers_) and enter `8.8.8.8` **and/or** `8.8.4.4` (the second one is an alternative). Restart your router and you should be using Google's public DNS servers!

TWC may put a limit on the download, or stream, speed that you can download from sites like YouTube, Twitch, Netflix and Hulu. Each time you open a video, your computer connects to a server, one that TWC has inherently throttled. Luckily, there is an easy fix to this problem. You'll need to block the primary connection that is requested. It will then request the default, faster, server (which will speed up the download speed tremendously).

There is an short, easy method of adding this IP block using the command prompt and a longer, more user interface friendly version. They both do the same thing – hope you can follow one of them.

> Check out [which browser is best]({% post_url reviews/2016-01-01-browsers %}) for speed and performance.

## Short version

Start -> type `cmd`
  
![Open cmd.exe from windows 7](https://i.imgur.com/iSDNPAV.png)
  
Type the following into the command prompt:
  
`netsh advfirewall firewall add rule name="TWC SUCKS" dir=in action=block remoteip=173.194.55.0/24,206.111.0.0/16 enable=yes`
  
Hit enter (You should get a confirmative &#8216;Ok.')
  
![Hit enter to get a confirmation message](https://i.imgur.com/3rvH6Xt.png)
  
That's it. Now it should default to the faster IP when requesting certain sites.

> Note: to undo this, type the following:
  
> `netsh advfirewall firewall delete rule name="TWC SUCKS"` 

## Long version

Start -> type `firewall`
  
![type firewall into start menu](https://i.imgur.com/Zo8HQFo.png)
  
Click InBound Rules (top left)
  
![inbound rules](https://i.imgur.com/L2JDXcG.png)
  
Click new rule
  
![Click new rule](https://i.imgur.com/rbxj94X.png)
  
Check custom -> next
  
![Select custom radio button](https://i.imgur.com/srk7Z0W.png)
  
Check all programs -> next
  
![Select All programs and hit next](https://i.imgur.com/cPePvWF.png)
  
Leave the default settings -> Next
  
![](https://i.imgur.com/8bdpjm8.png)
  
Under REMOTE IP addresses, check These IP addresses -> Add:
  
`173.194.55.0/24 206.111.0.0/16`
  
![](https://i.imgur.com/Vx6CKd1.png)
  
Next
  
Block the connextions -> Next
  
![](https://i.imgur.com/fnPrPr4.png)
  
Keep Domain, Private and Public all checked -> Next
  
![](https://i.imgur.com/4fMNM2i.png)
  
Give it a proper name and description -> Finish
  
![](https://i.imgur.com/z3OqYyA.png)