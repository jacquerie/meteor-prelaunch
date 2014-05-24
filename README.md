# meteor-prelaunch #

**meteor-prelaunch** is an application that lets you announce your future
project and collect emails of interested customers. It's written in JavaScript
using the [Meteor](http://www.meteor.com/) framework. This project is a fork
of [**mongolab-meteor-leadcapture-app**](https://github.com/FrozenRidge/mongolab-meteor-leadcapture-app) by FrozenRidge.

![Preview](/detail.png?raw=true "Preview")

## Features ##

* Design ~~inspired~~ blatantly stolen from Bootstrap's [Narrow marketing](http://getbootstrap.com/2.3.2/examples/marketing-narrow.html).
* Admin login with Github.
* MIT licensed.

## Installation ##

1. Install meteor.js: `$ curl https://install.meteor.com | sh`
2. Clone this project: `$ git clone https://github.com/jacquerie/meteor-prelaunch.git`
3. Move in the project directory: `cd meteor-prelaunch`
4. Edit `ADMIN_USERS` (line 6 in `app.js`) so that it contains your Github username(s)
5. Deploy to meteor.com: `meteor deploy --password APPNAME.meteor.com` where `APPNAME`
is your app's name, entering a new password when prompted.
6. Click on the Github button in the low left corner and register your new application
following the popup instructions.

## TODO ##

* Incoming email addresses are checked against a complicated Regex to ensure that they
are valid. I agree with [David Celis](http://davidcel.is/blog/2012/09/06/stop-validating-email-addresses-with-regex/) that this is the wrong approach: I'd rather use
Kicksend's [mailcheck](https://github.com/Kicksend/mailcheck).

* The admin view needs pagination. Currently no official package offers pagination,
but there's some unofficial support using packages from [Atmosphere](https://atmosphere.meteor.com/).

