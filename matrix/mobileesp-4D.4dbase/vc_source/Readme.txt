//%attributes = {"lang":"en"} comment added and reserved by 4D.
// ------------------------------------------------------
// Porting of mobilesp to 4D
// Copyright 2014 Lutz Epperelein 
// ------------------------------------------------------
// Copyright 2010-2013, Anthony Hand
// File version 2013.08.01 (August 1, 2013)
//      Updates:
//      - Updated DetectMobileQuick(). Moved the 'Exclude Tablets' logic to the top of the method to fix a logic bug.
//
// File version 2013.07.13 (July 13, 2013)
//      Updates:
//      - Added support for Tizen: variable and DetectTizen().
//      - Added support for Meego: variable and DetectMeego().
//      - Added support for Windows Phone 8: variable and DetectWindowsPhone8().
//      - Added a generic Windows Phone method: DetectWindowsPhone().
//      - Added support for BlackBerry 10 OS: variable and DetectBlackBerry10Phone().
//      - Added support for PlayStation Vita handheld: variable and DetectGamingHandheld().
//      - Updated DetectTierIphone(). Added Tizen; updated the Windows Phone, BB10, and PS Vita support. 
//      - Updated DetectWindowsMobile(). Uses generic DetectWindowsPhone() method rather than WP7.
//      - Updated DetectSmartphone(). Uses the detectTierIphone() method.
//      - Updated DetectSonyMylo() with more efficient code.
//      - Removed DetectGarminNuvifone() from DetectTierIphone(). How many are left in market in 2013? It is detected as a RichCSS Tier device.
//      - Removed the deviceXoom variable. It was unused.
//      - Added detection support for the Obigo mobile browser to DetectMobileQuick().
//
//
//
// LICENSE INFORMATION
// Licensed under the Apache License, Version 2.0 (the "License");
// you may not use this file except in compliance with the License.
// You may obtain a copy of the License at
//        http://www.apache.org/licenses/LICENSE-2.0
// Unless required by applicable law or agreed to in writing,
// software distributed under the License is distributed on an
// "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
// either express or implied. See the License for the specific
// language governing permissions and limitations under the License. 
//
//
// ABOUT THIS PROJECT
//   Project Owner: Anthony Hand
//   Email: anthony.hand@gmail.com
//   Web Site: http://www.mobileesp.com
//   Source Files: http://code.google.com/p/mobileesp/
//
//   Versions of this code are available for:
//      PHP, JavaScript, Java, ASP.NET (C#), and Ruby
//
// *******************************************
