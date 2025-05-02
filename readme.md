**Mark4 DCC Wi-Fi Throttle**

 [Mark4 Throttle](mark4.png) 

A model train diesel cab:

*   MicroPython / Raspberry Pi PICO W

	All code written in MicroPython and tested on a Raspberry Pi PICO W. Uses Peter Hinch's NanoGui to drive a WaveShare RGB OLED display. Makes extensive use of asyncio and event-style coding to handle all hardware and communications.
    
*   Speaks WiThrottle protocol
	
    Tested against JMRI's WiThrottle server. The intent is to also support the DCC-EX native command set.
    
*   8-notch throttle lever

	The throttle control makes use of a potentiometer with detents that simulates the 8 notch throttle found on early generation diesel locomotives.
    
*   Brake lever

	A brake function is also available using a potentiometer that, through the software, can emulate a progressive (analog) engine brake with four steps defined. Horn and Bell buttons are also provided.
    
*   Horn and Bell buttons

*   Direction switch

	Selects Forward, Reverse, Idle

*   Two assignable function buttons

	Two user-assignable function buttons are also provided. Typical use would be for headlights and ditchlights.
    
*   5-way switch for menu navigation

	The throttle uses a 5-way joystick-style button/switch for menu navigation. The menu system allows for acquiring/releasing locomotives (roster provided by JMRI), calibrating throttle and brake pots, and toggling AP 'hotspot' mode (see below).
    
*   Emulated momentum and braking for “dumb” decoders.

	When used with 'dumb' (two or four function decoders), locomotive momentum and braking are emulated via software. Both momentum and braking can be adjusted or turned off.
    
*   Custom μPython firmware w/ mDNS

	The Mark4 Throttle does use a custom μPython firmware, which has been customized to use cbrand's pure Python mdns implementation. This is used to allow for discovery of withrottle servers.
    
*   Can boot to AP Wi-Fi to allow phone or tablet input to configure throttle

	The Mark4 Throttle does not incorporate a keypad. Instead, the throttle can optionally boot to an AP 'hotspot' mode and then provides a web interface for a phone / tablet or computer to enter different configuration parameters such as wi-fi ssid/password, loco roster data not held by JMRI, and other related config info.
    
*   OLED RGB display

	Displays throttle and brake settings, bell, acquired locos, other menu-related options, and warnings such as 'No Wi-FI Acquired', 'No WiThrottle Servie', 'No Loco Acquired', etc.

    
Code will be posted here in short order, but not today. 
