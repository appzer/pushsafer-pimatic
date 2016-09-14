pimatic-pushsafer
=======================

![Pushsafer](https://www.pushsafer.com/de/assets/logos/logo.png)

A plugin for sending [pushsafer.com](https://www.pushsafer.net/) notifications in pimatic.

Forked from and original created by: [thexperiments](https://github.com/thexperiments/pimatic-pushover)

Pushsafer make it easy and safe to get push-notifications in real time on your
- Android device
- iOS device (incl. iPhone, iPad, iPod Touch)
- Windows Phone & Desktop
- Browser (Chrome & Firefox)

Configuration
-------------
You can load the backend by editing your `config.json` to include:

    {
      "plugin": "pushsafer",
      "privatekey": "Your20CharPrivateKey"
    }

in the `plugins` section. For all configuration options see 
[pushsafer-config-schema](pushsafer-config-schema.coffee)

Currently you can send pushsafer notifications via action handler within rules.

Example:
--------

titleTokens, messageTokens, sound, device, icon, vibration

    if it is 08:00 push title:"Good morning!" message:"Time to get out of bed!" sound:"11" device:"312" icon:"4" vibration:"2"

in general: if X then push

    title:"title of the push notification" message:"message of the notification" sound:"11" device:"312" icon:"4" vibration:"2"

Find API description here at [pushsafer api](https://www.pushsafer.com/de/pushapi) to set up your push notification!
