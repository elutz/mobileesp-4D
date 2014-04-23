# mobileesp for 4D v13

## Description
mobileesp for 4D is a port of [mobileesp](http://www.mobileesp.com) to 4D. You can use it in a webserver process to detect the usage of mobile devices on the client side.

## Contents

* The [Components] folder contains the "mobileesp-4D.4dbase" component suitable for installation in any [4D v13](http://www.4d.com/products/4dv13.html) database.
* The [matrix] folder contains the component source code.

## Usage

Install the component. 

It provides the following public methods:
* initDetection 
* getIsIPhone
* getIsTierIphone
* getIsTierTablet

At first you have to call the method *initDetection* of the component, providing the two parameters `userAgent` and `httpAccept` extracted out of the http headers. Afterwards you can use the getter methods to retrieve the device information.

### getIsIPhone
Return whether the device is an Iphone or iPod Touch

### getIsTierIphone
Return whether the device is in the Iphone Tier. This means devices which can
     *   display iPhone-optimized web content.
     *   Includes iPhone, iPod Touch, Android, Windows Phone 7 and 8, BB10, WebOS, Playstation Vita, etc.

### getIsTierTablet
Return whether the device is in the Tablet Tier. This means the new generation of 
     *   HTML 5 capable, larger screen tablets.
     *   Includes iPad, Android (e.g., Xoom), BB Playbook, WebOS, etc.

## TODO
Completing the port, especially `detectTierRichCss` and `isTierGenericMobile`.
