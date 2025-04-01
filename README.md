# MotionEyeOS-Zero2W
 Fork of MotionEyeOS for the Raspberry Pi Zero 2 W.

For Wireless configuration, open Notepad++ and set to UNIX mode,
change "Save as type" to All, and create a wpa_supplicant.conf file 
with the text below, adapted for your network SSID, password and region. 
Add this file to the system config files after flashing MotionEyeOS to 
your SD card with Balena Etcher.

        country=CA
        update_config=1
        ctrl_interface=/var/run/wpa_supplicant
        
        network={
            scan_ssid=1
            ssid="MyWiFiSSID"
            psk="S3cr3tp@$$w0rc|"
        }
