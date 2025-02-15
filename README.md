# Meshtatic-default-setup

### Meshtastic go to Chromium Browser folder (snap block usb device)
```shell
cd /snap/chromium/current/usr/lib/chromium-browser
```
### Meshtastic start chromium browser
```shell
./chrome &
```
-   go to: https://flasher.meshtastic.org/ and flash your device :)
  
-   read more: https://meshtastic.org/docs/getting-started/flashing-firmware/esp32/web-flasher/

### Meshtastic set your region (Serial) CLI
```shell
meshtastic --set lora.region EU_868
```
-   read more: https://meshtastic.org/docs/getting-started/initial-config/

### Meshtastic set nickname and shortname (Serial) CLI
```shell
meshtastic --set-owner 'your node name' --set-owner-short  'NODE'
```
-   read more: https://meshtastic.org/docs/configuration/radio/user/

### Meshtastic set Network Configuration (Serial) CLI
```shell
meshtastic --set network.wifi_ssid "WLAN_name" --set network.wifi_psk "WLAN_Passwort" --set network.wifi_enabled 1
```
-   read more: https://meshtastic.org/docs/configuration/radio/network/


### Meshtastic set fixed position (Serial) CLI
```shell
meshtastic --set position.fixed_position true --setlat 37.8651 --setlon -119.5383
```
-   read more: https://meshtastic.org/docs/configuration/radio/position/


### Meshtastic set position minimum distance (Serial) CLI
```shell
./meshtastic --set position.broadcast_smart_minimum_distance 0
```
-   integer (meters) Default of 0 is 100 Meters 
-   read more: https://meshtastic.org/docs/configuration/radio/position/
