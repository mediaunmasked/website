---
title: How to do FPV on your phone
date: 2016-02-15 00:00:00 Z
categories:
- tutorials
image: "/assets/2016/02/nrGgCUM.jpg"
excerpt: Discover how to affordably fly FPV RC quadcopters on your phone with an app,
  a wire, and a module.
---

## Radio controlled first person view

We live in a fantastic time (compared to the past, not the future), and part of what makes this year so great is the ability to pilot an aircraft the size of a tarantula for under $50.

One of the fastest growing areas of technology is _drones_, or RC helicopters. They, and other RC vehicles, have been around for many years, but have recently grown in popularity with the combined implementation of affordability, ease-ability, and on-board cameras for filming or first-person-view flight.

Although I've had my fair share of RC as a child, these introductions also piqued my interest as an adult. So, I built a crude tricopter out of wood and slapped a GoPro on it and became one of the other millions of people to upload their shaky footage to YouTube.

![FPV Youtube search results](https://i.imgur.com/e9NbrR9.jpg)

While getting a bird's eye view of your house is fun, I began to further explore the idea of flying with a live video feed like I've seen other people do. I later bought a pair of [Fatshark FPV video goggles](http://amzn.to/1mz8U6G) that basically act as a monitor (attached to your face) with a dedicated location for proprietary video receiver and head-tracking modules — neat, huh?

## Hardware & software

<div class="row">
  <div class="col s12 m4">
    <img src="https://i.imgur.com/mfclBWb.jpg" alt="LaserBGC wireless USB module receiver for Fatshark FPV headset goggles" />
  </div>
  <div class="col s12 m8">
    <p>Today, technology is rampant and the amount of different phones and drones is staggering. Phones range from $20 to $700+ and all offer similar<i>ish</i> features. The same can be said about RC multirotor helicopters, but they seem to be dropping in price much faster than phones.</p>
    <p>Regardless, to get a decent setup, you can easily spend upwards of <b>$1000+</b> to get in the sky. <i>Or not</i>. Since phones are basically a tiny display, why not use it to fly a quadcopter? Here's a list of items, software, etc. I'll be using to <b>get FPV on a phone</b> for much cheaper.</p>
    <blockquote>
      <b>Update:</b> LaserBGC now has a receiver module that plugs directly into your phone (phone still needs to support OTG), removing the need for a dedicated OTG cable.
    </blockquote>
  </div>
</div>

<ul class="collection with-header">
  <li class="collection-header">
    <h3>
      Video Rx (Receiver)
    </h3>
  </li>
  
  <li class="collection-item">
    Android phone with <a href="https://play.google.com/store/apps/details?id=com.homesoft.otgtroubshooter&#038;hl=en">OTG support</a>
  </li>
  <li class="collection-item">
    <a href="http://amzn.to/1mzcfCK">Video receiver module</a>
  </li>
  <li class="collection-item">
    <a href="http://laserbgc.com/index.php?route=product/product&#038;product_id=82">Video receiver USB module</a> & <a href="http://amzn.to/1HwM5El">OTG cable</a><br />or<br /><a href="http://laserbgc.com/index.php?route=product/product&#038;path=67&#038;product_id=83">Modular receiver for Android</a>
  </li>
  <li class="collection-item">
    <a href="http://amzn.to/1HwLYZl">Google Cardboard</a> or <a href="http://amzn.to/2nCrmRm">VR Box</a>
  </li>
  <li class="collection-item">
    <a href="https://play.google.com/store/apps/details?id=labsp.android.viewer">FPViewer</a> App
  </li>
  <li class="collection-item">
    <b>Optional:</b> <a href="http://amzn.to/1HwMgze">Fatshark diopter corrective lenses</a> (if you're nearsighted)
  </li>
  <li class="collection-header">
    <h3>
      Video Tx (Transmitter)
    </h3>
  </li>
  
  <li class="collection-item">
    <a href="http://amzn.to/1mzeC8o">Video transmitter</a>
  </li> 
    
  <li class="collection-item">
    <a href="http://amzn.to/1PTRmhv">Video camera</a>
  </li>
  <li class="collection-item">
    <b>Optional:</b> <a href="http://amzn.to/20SE0sP">Battery for video Tx</a><br />Otherwise, solder into your power distribution from your vehicle
  </li>
  <li class="collection-item">
    <b>Optional:</b> <a href="http://amzn.to/20SExLf">Lipo battery charger</a> and <a href="http://amzn.to/20SECi7">protective bag</a>
  </li>
</ul> 
    
## See it in action
    
<img src="https://i.imgur.com/et3BG5o.jpg" alt="FPV quadcopter racing on your phone" />
    
### Transmitter
    
Make sure the video transmitter and receiver you get run on the same frequency. In this example, you'll need to get a Fatshark-fitted module to fit on the USB module. I use the 1.3GHz bandwidth so it penetrates structures or 5.8GHz for distance. Also, ensure that you have the right voltage battery for the job. 11.1V (3 cell) is common.
    

<img src="https://i.imgur.com/YCx6qTB.jpg" alt="FPV video transmitter battery" /><img src="https://i.imgur.com/mTeMVMi.jpg" alt="FPV video transmitter battery" />

First, make sure the video transmitter has an antenna on it before proceeding. I've heard it can fry the insides if it doesn't have one on the transmitter. Not including an antenna on the receiver is okay, but it's got reduced effectiveness. Simply plug in the battery to the video transmitter and it should be on.

Some quads power the transmitter/camera with the quad's main battery, which certainly simplifies it. These things can get warm, so when you place it on a vehicle, be sure to allow for some air flow. Racing quadcopters are usually cut to an optimized size and it should be obvious where to place the battery.
    
If you're powering the transmitter with a separate power supply, connect the battery to the transmitter and the transmitter to the video output port on the camera.

### Receiver

<img src="https://i.imgur.com/pVkuLDT.jpg" alt="Video receiver for FPV on your phone" /><br /> 
  
<div class="center-align">
  <video autoplay loop>
    <source type="video/webm" src="https://i.imgur.com/2SvN1os.webm">
    <source type="video/mp4" src="https://i.imgur.com/2SvN1os.mp4">
  </video>
</div>

If you bought the USB adapter instead of the one for your phone, just plug the USB module into your phone with the OTG cable and open the FPView (or similar) app. Otherwise, plug it in and start flying!

<img src="https://i.imgur.com/09N6udO.jpg" alt="OTG on the go cable adapter" />

Tada! Now you have an external monitor that you can use to fly FPV and use to record as an on-board camera. With a phone head strap like Google Cardboard or comparable devices like VR Box, you can either fly with it on your head or looking down at the screen.

## Cardboard

Luckily, Google implemented some free plans so anyone can turn their phone into a (virtual reality) headset! With the help of Chinese manufacturers and free shipping, you can get a precut kit with the magnet, eye pieces, and other required parts on ebay or amazon.

<img src="https://i.imgur.com/eFjjizt.jpg" alt="Goole Cardboard FPV setup with phone as monitor" />

Nothing particularly new or revolutionary, but by using your phone and cardboard, you're saving $300+ that would have been spent on a dedicated set of video goggles. I'm pretty sure the latency is comparable; it is certainly responsive enough to be able to fly with. But your phone can also call, text, game (virtual reality), etc.

<div class="center-align">
  <video autoplay loop>
    <source type="video/webm" src="https://i.imgur.com/oXilp86.webm">
    <source type="video/mp4" src="https://i.imgur.com/oXilp86.mp4">
  </video
</div>>