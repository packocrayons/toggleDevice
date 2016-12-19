##Toggle Device Script

Use xinput --list to get the number of the device that you would like to toggle, then call toggle_device with that number.

For example (on my machine):
xinput --list
⎡ Virtual core pointer                    	id=2	[master pointer  (3)]
⎜   ↳ Virtual core XTEST pointer              	id=4	[slave  pointer  (2)]
⎜   ↳ Atmel Atmel maXTouch Digitizer          	id=10	[slave  pointer  (2)]
⎜   ↳ ETPS/2 Elantech Touchpad                	id=14	[slave  pointer  (2)]
⎣ Virtual core keyboard                   	id=3	[master keyboard (2)]
    ↳ Virtual core XTEST keyboard             	id=5	[slave  keyboard (3)]
    ↳ Power Button                            	id=6	[slave  keyboard (3)]
    ↳ Video Bus                               	id=7	[slave  keyboard (3)]
    ↳ Power Button                            	id=8	[slave  keyboard (3)]
    ↳ Sleep Button                            	id=9	[slave  keyboard (3)]
    ↳ USB2.0 HD UVC WebCam                    	id=11	[slave  keyboard (3)]
    ↳ Asus WMI hotkeys                        	id=12	[slave  keyboard (3)]
    ↳ AT Translated Set 2 keyboard            	id=13	[slave  keyboard (3)]

A call to toggleDevice 10 will disable the touchscreen (maXTouch Digitizer)
