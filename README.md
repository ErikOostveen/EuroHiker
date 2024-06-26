### Index

<a href="#eurohiker">EuroHiker</a><br>
<a href="#assemble1">Let's Assemble! - Part I - EuroHiker PCB 1 of 2</a><br>
<a href="#assemble2">Let's Assemble! - Part II - EuroHiker PCB 2 of 2</a><br>
<a href="#divinginto1">Diving into the EuroHiker module | Setup</a><br>
<a href="#divinginto2">Diving into the EuroHiker module | Testing</a><br>
<a href="#supercollider">SuperCollider (audio synthesis)</a><br>
<a id="eurohiker"></a>
# EuroHiker

The EuroHiker module is designed to provide a programmable platform capable of executing various functions, fitting seamlessly into the world of EuroRack where modules are typically fine-tuned to excel in their designated tasks.

The EuroHiker module is the core module in the [STEAM Modular series](https://www.erikoostveen.co.uk/SteamModular.html)

![EuroHiker_With_Exp_Cable](https://github.com/ErikOostveen/EuroHiker/assets/40121318/e78d3542-780f-490a-b9b9-739aca90ba37)

The EuroHiker module is based on the popular (Linux) Unihiker single board computer by [DFRobot](https://www.dfrobot.com/product-2691.html)

The UniHiker board comes standard with WiFi/Bluetooth, Light Sensor, Microphone, Accelerometer sensor, Gyroscope sensor, Buzzer, MicroSD card slot and Various I/O connectivity (PWM, ADC, I2C, UART, USB, SPI)

The EuroHiker module adds to this already impressive list of features MIDI IN/OUT, Gate IN/OUT, Control Voltage IN/OUT, two push buttons, a Rotary Encoder with built in Red/Green/Blue LEDs plus another push button. The module also has an ON/OFF switch - and last but not least, offers an expansion interface (26pins) for you to experiment and interact with the EuroHiker module through your own designs!

Download the [EuroHiker Visual Summary (PDF | 19Mb) here](https://github.com/user-attachments/files/15792319/EuroHiker_OnePager.pdf)

Module Specs
<br>• 3U/20HP = approx. H128mm x W101mm
<br>• Depth approx. 40mm
<br>• +12V = 600mA, -12V = 25mA, +5V = 0mA

The EuroHiker module is designed to provide a programmable platform capable of executing various functions, fitting seamlessly into the world of EuroRack where modules are typically fine-tuned to excel in their designated tasks.

The EuroHiker module, on the other hand, empowers you to navigate through folders containing Python programs, each leveraging the module's extensive feature set.

The idea is to have the flexibility to explore numerous concepts, allowing you to test them before deciding whether to further develop them using another development board or to retain them with
<a id="assemble1"></a>
# Let's Assemble! - Part I - EuroHiker PCB 1 of 2
[PCB Link](https://github.com/ErikOostveen/EuroHiker/tree/main/2%20-%20PCB_1_of_2__UniHiker_Board_and_FrontPanel_Components)<br>
The first part, of two, in assembling the EuroHiker module, is to gather all required components. I had the PCB, which houses the front panel's components, partially populated becasue I had some of the parts in stock. See overview below:

![pcb_1_overview](https://github.com/ErikOostveen/EuroHiker/assets/40121318/3e42fe15-b6ab-46be-93e7-86d1de6bcb39)

### Step A
Partially populated PCB. 
What follows are the suggested steps to building the EuroHiker module. I have also included links to some of the components - these are suggestions also. Sometimes links come back "blocked"; in that case just copy/paste the link into your browser.   

### Step B
Start with the Edge Connector (BBC micro:bit).<br>
Link: https://kitronik.co.uk/products/4148-edge-connector-header-for-bbc-microbit<br><br>
![big_connector2](https://github.com/ErikOostveen/EuroHiker/assets/40121318/a196fd32-167f-4dd2-93af-0fca1281fff7)

### Step C
Solder the 2 Right-Angled 2Pin Sockets.<br> 
Link:https://www.lcsc.com/product-detail/Female-Headers_CONNFLY-Elec-DS1024-1x2R2_C7509534.htmld<br>
These sockes are not mandatory; you can solder wires directly from this PCB to the USB breakout boards (mentioned further down in the steps).<br><br>
![sockets](https://github.com/ErikOostveen/EuroHiker/assets/40121318/1c3608f7-a3e0-456e-986a-cee843d94a3a)

### Step D
Solder the 6 3.5mm jack sockets. Keep in mind; the 2 MIDI sockets are STEREO sockets (Green on image) the remaining 4 are MONO (Black on the image).
By far the best place to get these jack sockets is THONK.<br>
Link: https://www.thonk.co.uk/shop/3-5mm-jacks/<br><br>
![JACKS](https://github.com/ErikOostveen/EuroHiker/assets/40121318/659e82f4-a1bd-4916-b729-4ecb5da68780)

### Steps E & F
The tallest components go last (we'll get to the LEDs later); "E" first:<br>
1 x Miniature Toggle (the Power) Switch<br>
Link: https://www.digikey.co.uk/en/products/detail/e-switch/100SP1T1B4M2QE/378824?s=N4IgTCBcDaIIwAYEGUAKcAqcBCAWAsmAIoCiIAugL5A<br>
2 x Push Buttons (Left/Right) (6.2x6.2x13mm)<br>
Link: https://www.lcsc.com/product-detail/Tactile-Switches_Diptronics-DTS-66K-V_C141877.html
Then "F":<br>
1 x Rotary RGB Encoder<br>
Link: https://uk.robotshop.com/products/rotary-rgb-encoder-illuminated<br><br>
![toggle_sw_buttons_encoder](https://github.com/ErikOostveen/EuroHiker/assets/40121318/ffab539d-409b-4091-8817-ebc3274af27b)

### Step G
Time the flip the board around and solder the 3 sockets for connectivity to the 2nd board.<br>
1 x 4PIN Socket (i.e. 2 x 2Rows)<br>
Link: https://www.lcsc.com/product-detail/Female-Headers_Liansheng-FH-00221_C2685206.html<br>
2 x 20PIN Sockets (i.e. 2 x 10Rows)<br>
Link: https://www.lcsc.com/product-detail/Female-Headers_Liansheng-FH-00088_C2685085.html<br><br>
![Sockets_Rear_pcb_1](https://github.com/ErikOostveen/EuroHiker/assets/40121318/1e4bb87e-2a64-4515-8cf3-2d62b1d0d11e)

### Step H
We need to break-out the UniHiker's USB-A and USB-C ports with two short "USB patches". The USB-C port (the smallest connecter at the top of the UniHiker board) will be used to power the UniHiker. The USB-A port connects to the MIDI interface on the 2nd PCB.<br>
* USB-C to PCB:<br>
1 x USB-C socket breakout<br>
Link: https://www.digikey.co.uk/en/products/detail/adafruit-industries-llc/5180/15287551?s=N4IgTCBcDaIIwFYwA4C0C7IAyoHIBEQBdAXyA<br>
1 x 2Pin 2.5mm pitch<br>
Link: https://www.lcsc.com/product-detail/Pin-Headers_chxunda-XDZ254-1-14-Z-2-5-G1_C18905855.html<br>
Wire Colours: Red = + (5V), Blue = GND (Ground)<br>
* USB-A to PCB:<br>
1 x USB-A socket breakout<br>
Link: https://cpc.farnell.com/clever-little-box/cie-yy27/usb-2-0-a-plug-breakout-board/dp/CN22559<br>
1 x 2pin 2.5mm pitch<br>
Link: https://www.lcsc.com/product-detail/Pin-Headers_chxunda-XDZ254-1-14-Z-2-5-G1_C18905855.html<br>
Wire Colours: Green = Data Negative (D-), White = Date Positive (D+)<br><br>
The PCB's image on the right illustrates how these "USB patches" will connect into the UniHiker (later)<br><br>
![two_usb_patches](https://github.com/ErikOostveen/EuroHiker/assets/40121318/eeba7c67-7dad-46f1-87cd-5cd7c5ac348d)

### Step I
Ok, time to put the PCB aside and focus on the UniHiker board itself!<br>
I1: connect 3 white wires/patches* to the UniHiker: P21, P22 & P23 (there's text on the UniHiker board to identify these ports). (*) these come with the UniHiker board<br>
I2: Power-up the UniHiker board by connecting the included USB cable to your computer. Let it boot - and Select "English" from the menu.<br> 
I3: After a reboot, long-press the screen (or home button) to enter the menu.<br>
I4: Launch a browser on your computer and enter 10.1.2.3 as the URL. Go to "Network Settings".<br>
I5: Use the scan/drop-down menu to find your home's WiFi network and enter its password.<br>
I5: Use the scan/drop-down menu to find your home's WiFi network and enter its password.<br>
I6: Once connected, make a note of the IP address (192.168.0.246 in this example).<br><br>
![boot](https://github.com/ErikOostveen/EuroHiker/assets/40121318/07e6a15c-0023-4dfb-96d1-7cc66f642eb9)

I7: Remove the protective film from the UniHiker's top mounting hole and have a short nylon M3 screw at hand.<br>
I8: Feed the 3 white wires through the PCB's cutouts.<br>
I9: Now, carefully insert the UniHiker into the Edge Connector - carefully guiding the wires!<br>
I10: Secure the UniHiker to the PCB with the M3 screw.<br><br>
![UniHiker_on_PCB](https://github.com/ErikOostveen/EuroHiker/assets/40121318/a7ee253b-5628-488c-ad0f-91344c755c2f)

### Steps J, K & L
J1: Insert all 7 LEDs, but DON'T solder them yet! Push them in as far as possible. We"ll get back to these later.<br>
K1: Put the washers in place. I use 2 for each of the 3.5mm jacks; this way, the front panel sits comfortably over the top of the UniHiker's screen.<br>
Have a look at these colouful Jack nuts for inspiration: https://www.thonk.co.uk/shop/bananuts/<br>
K2: Fit the front panel.<br>
My UK frontpanel supplier of choice is: https://www.meface.co.uk/  
L1: Place & Fasten all nuts. Do not "over tighten" the nuts or you'll break the screen (potentially). Fasten the Encoder's knob.<br> 
J2: Back to the LEDs. Feed the LEDs through the holes and aim to get them flush with the front panel. Now you can solder them.<br><br>
![steps_j_k_l](https://github.com/ErikOostveen/EuroHiker/assets/40121318/b6655be5-4528-49a5-a647-dd798c6526ae)

### Completing the first part
Finally, connect both USB patches. Make sure to, carefully, tuck the wires away.<br><br>
![connect_usbs](https://github.com/ErikOostveen/EuroHiker/assets/40121318/2e61942f-8241-4a64-8679-40bd48bb93db)<br>
Cool!, you completed the first part to building the EuroHiker module!
<a id="assemble2"></a>
# Let's Assemble! - Part II - EuroHiker PCB 2 of 2
[PCB Link](https://github.com/ErikOostveen/EuroHiker/tree/main/4%20-%20PCB_2_of_2__Active_Components_and_Outboard_Connectivity)
### Step M
The 2nd PCB is super easy to build. Lets summarise the components (see image further below)<br>
M1: Partially populated PCB. In fact, this is simply a one-side-only populated PCB; it's quite a bit cheaper this way than having both sides populated.<br> 
M2: 1 x 16pin (2x8pins) Male Header<br>
Link: https://www.lcsc.com/product-detail/IDC-Connectors_BOOMELE-Boom-Precision-Elec-2-54-2-8P_C3406.html<br>
M3: 1 x 26pin (2x13pins) Male Header<br>
Link: https://www.lcsc.com/product-detail/IDC-Connectors_Megastar-ZX-IDC2-54-2-13PZZ_C7501247.html<br>
M4: 3 strips of 14pins each at 2.5mm pitch<br>
Link: https://www.lcsc.com/product-detail/Pin-Headers_chxunda-XDZ254-1-14-Z-2-5-G1_C18905855.html<br>
M5: 14 x 2.54mm Jumper (female)<br>
Link: https://www.mouser.co.uk/ProductDetail/Harwin/M7582-05?qs=ulE8k0yEMYZPqg5dozLsXw%3D%3D<br><br><br>
![2nd_pcb](https://github.com/ErikOostveen/EuroHiker/assets/40121318/be471286-f7ca-466c-9aff-f68617fdec46)

### Step N
Solder the 2 headers and the 3 strips. Connect all 14 jumpers to the default position (to the left - as shown on the image below)<br><br>
![2nd_pcb_soldered](https://github.com/ErikOostveen/EuroHiker/assets/40121318/78fcef35-a350-45f2-a784-3ddfc8218a69)

### Step O - Pairing the PCBs!
It's time to link the two PCBs. Grab the PCB/Frontpanel from Part I and connect the 3 white wires (P21, P22, P23). These three wires control the rotary encoder's RGB LEDs - with the jumpers for P21, P22 & P23 in the default position that is. More about these jumpers later<br><br>
![pairing_PCBs_1](https://github.com/ErikOostveen/EuroHiker/assets/40121318/6becce26-05a0-4715-a0b1-b7b00d2972c1)

### Step P
Carefully push the 3 headers (the pins) into their opposite sockets. Make sure not to pierce any of the wires! - I managed to do this and only found out after powering up the module - luckily there was no electrical damage, but, of course, it could have damaged the board or, worse, the Unihiker module(!).<br><br>
![pairing_careful](https://github.com/ErikOostveen/EuroHiker/assets/40121318/355feb8c-9664-4e2e-87d9-b8bf39be21ba)

### Step Q
It's time to power up the module. Make sure the EuroHiker's toggle switch is set to the OFF position (facing away from the Power LED).<br><br>
Connect the EuroRack power cable from your EuroRack power supply to the EuroHiker module:<br><br>
![connect_power_cable](https://github.com/ErikOostveen/EuroHiker/assets/40121318/bb6dccaf-81da-43d8-9269-bb5523975e5a)

Mount the EuroHiker module into your EuroRack setup or desktop case and throw the EuroHiker's toggle switch. The YouTube video below shows the bootup of the EuroHiker module:<br><br>
<a href="http://www.youtube.com/watch?feature=player_embedded&v=zgOlJGRqT2I" target="_blank"><img src="http://img.youtube.com/vi/zgOlJGRqT2I/0.jpg" width="400" border="1" /></a>

Notice that the two Yellow MIDI IN/OUT LEDs blink for a second and then switch off. The Power LED switches ON and on a newly built module, the CV OUT LED switches ON also. We will go through all ports, buttons and rotary encoder next including CV OUT.<br><br>
For now, long-press the screen and the menu should appear. Tap the screen, navigate around, to make sure that the touch screen works fine.
<a id="divinginto1"></a>
# Diving into the EuroHiker module | Setup
We have come a long way building the module! Now, lets make sure that all is working as it should.

### EuroHiker software

[Go to the STEAM Modular Google Drive](https://drive.google.com/drive/folders/14qjXZDC-lNFwKs0wiuWyef0XtvS9_sYN?usp=sharing)

Go to the <strong>EuroHiker</strong> directory and download the EuroHiker archive called:
```
EuroHiker_<Month>_<Day>_<Year>.tar
```
Save it somewhere on your computer - we will revisit this arhive later.

### IP Address of the EuroHiker module

In step I6, we found out about the UniHiker's WiFi IP address. If you lost that info or you suspect that the IP address may have changed, then the following will help you find its IP address:<br>
1. Long press the screen
2. Navigate to "4-Network Info"
3. On the screen that follows, "Wireless: xxx.xxx.xxx.xxx" tells you the UniHiker's IP address (or EuroHiker rather)

### Remote Login (SSH & SFTP)

If you don't already have these remote login tools, then please;<br>
[Download PuTTY](https://www.putty.org/) - a free SSH and telnet client for Windows and ...<br>
[Download WinSCP](https://winscp.net/eng/index.php) - a free SFTP client and FTP client for Windows<br>

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

From the command prompt, enter:
```
cd /opt/unihiker/examples
rm -rf *
cd ..
```

Use WinSCP, or similar software, to SFTP into the EuroHiker.
The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

Copy the archive file you download earlier into the following directory:
```
/opt/unihiker
```
### Install software to get you started

Go back to the command prompt, enter:
```
pwd
# This should return: /opt/unihiker
# if not, enter: cd /opt/unihiker

ls -l *.tar
# This should return the .tar file you uploaded to the EuroHiker module
# In the example below, replace "EuroHiker_June_6th_2024.tar" for the filename of your .tar file

tar -xvf EuroHiker_June_6th_2024.tar
# In the output that follows, you can see that this archive populates the examples directory
# It also replaces the EuroHiker's default UniHiker splash screen for the STEAM Modular splash screen
# Lets reboot

sudo reboot now
```
Your EuroHiker now looks more "Eurohiker" after boot up.

Just so you know where to find the example files:
1. Long press the screen
2. Navigate to "2-Run Programs"
3. Navigate to "demo/"
4. This is the root directory of all current and future projects
   
This <strong>demo/</strong> directory accessible through the User Interface is the EuroHiker's <strong>/opt/unihiker/examples</strong> directory. It's the root directory you will go to time after time to work on your projects!
<a id="divinginto2"></a>
# Diving into the EuroHiker module | Testing
Now, we will walk through all Ports, LEDs the Rotary Encoder and Buttons.

Before we get started, please remember that the [UniHiker website](https://www.unihiker.com/) is your goto place to find out more about the EuroHiker's UniHiker board.

Another thing to remember is that all tests/programs below are written in Python.

### Rotary Encoder (LEDs)

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

From the command prompt, enter:
```
# TEST 1 (Individual LEDs ON/OFF):
cd /opt/unihiker/examples/100-EuroHiker/RGB_LEDs
python  test_RED_GREEN_BLUE_LEDs.py
# This should make the Red, Green and Blue LEDs inside the Rotary Encoder flash
# Press Ctrl+z to stop the program
# Note that after stopping this test program, a LED may still be on - this is fine.
# When you start programming yourself, you can make sure all LEDs are off when quiting a program.

# TEST 2 (Multiple LEDs | PWM) 
python PWM_P21_Red__P22_Green__P23_Blue.py
# Here we are "mixing" Red, Green and Blue - at different PWM rates or LED brightness so we get different colours
# Press Ctrl+z to stop the program
# Note that after stopping this test program, a LED may still be on - this is fine.
# When you start programming yourself, you can make sure all LEDs are off when quiting a program.
```

### Rotary Encoder (Turn & Press)

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

From the command prompt, enter:
```
# TEST 1 (Turn):
cd /opt/unihiker/examples/100-EuroHiker/ROTARYENCODER
python encoderTest.py
# Turn the Rotary Encoder's knob Clockwise.
# You should see "Counter: 1 ... 2 ... 3 etc." in your SSH terminal
# Turn the Rotary Encoder's knob Counter-Clockwise.
# You should see, at some point, "Counter: -1 ... -2 ... -3 etc." in your SSH terminal

# TEST 2 (Press):
# Press the Rotary Encoder's knob. You should see "Pressed" (many times)
# Press Ctrl+z to stop the program
```

### Left & Right Push Buttons

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

From the command prompt, enter:
```
# TEST LEFT
cd /opt/unihiker/examples/100-EuroHiker/PUSHBUTTONS
python test_push_buttons.py
# Press the LEFT button. 
# You should see "Left Push Button Pressed" in your SSH terminal (many times)

# TEST RIGHT
# Press the RIGHT button. 
# You should see "Right Push Button Pressed" in your SSH terminal (many times)
# Press Ctrl+z to stop the program
```

### Buzzer

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

From the command prompt, enter:
```
cd /opt/unihiker/examples/100-EuroHiker/BUZZER
python buzzer.py
# You should hear the EuroHiker's buzzer play a melody and stop
# Press Ctrl+z to stop the program
```

### Microphone

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

From the command prompt, enter:
```
cd /opt/unihiker/examples/100-EuroHiker/MIC
python mic.py
# You should see "Ambient volume = .." in the terminal window
# Make some loud noises - this should change the volume values shown
# Press Ctrl+z to stop the program
```

### Light Sensor

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

From the command prompt, enter:
```
cd /opt/unihiker/examples/100-EuroHiker/LIGHTSENSOR
python lightSensor.py
# You should see "Ambient light intensity: .." in the terminal window
# Cover the EuroHiker's right slit - this should change the light intensity values shown
# Shine your phone's torch into this slit and see how high the values become!
# Press Ctrl+z to stop the program
```

### MIDI IN/OUT | IN

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

Connect the MIDI OUT of a MIDI keyboard to the MIDI IN of the EuroHiker module (Type-A MIDI).<br>
Set the keyboard to MIDI Channel 1.

From the command prompt, enter:
```
# TEST - Receiving MIDI Data

# Install the py-midi library IF YOU HAVEN'T DONE THIS ALREADY (this is a one-off)
# Reference: https://github.com/edthrn/py-midi
pip3 install py-midi
# Install will take a while. You may see a warning message - but that's ok. You can ignore it.

cd /opt/unihiker/examples/100-EuroHiker/MIDI
python midiLib_RX.py
# Press a few keys. In your terminal window, you should see the MIDI note number and note velocity. 
# Also note the MIDI IN led blinking as you play the keyboard.
# When no MIDI is received, you see the occasional "None"
# Press Ctrl+z to stop the program
```

### MIDI IN/OUT | OUT

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

Connect the MIDI IN of a MIDI instrument to the MIDI OUT of the EuroHiker module (Type-A MIDI).<br>
Set the instrument to MIDI Channel 1. Select a patch (like piano for example).

From the command prompt, enter:
```
# TEST - Transmitting MIDI Data

# Install the py-midi library IF YOU HAVEN'T DONE THIS ALREADY (this is a one-off)
# Reference: https://github.com/edthrn/py-midi
pip3 install py-midi
# Install will take a while. You may see a warning message - but that's ok. You can ignore it.

cd /opt/unihiker/examples/100-EuroHiker/MIDI
python midiLib_TX.py
# Note the MIDI OUT led blinking.
# For this test, the .py program transmits a NOTE ON message (first blink)
# then it transmits a NOTE OFF message (second blink) and so on
# Press Ctrl+z to stop the program
```

### GATE IN/OUT | IN

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

Connect the Gate OUT of your analog instrument to the Gate IN of the EuroHiker Module.<br>
The Gate IN LED of the EuroHiker module should now blink in sync with the Gate OUT LED of your instrument.<br>

From the command prompt, enter:
```
cd /opt/unihiker/examples/100-EuroHiker/GATE_IN
python digital_in.py
# When the EuroHiker's Gate IN LED is ON, your terminal screen will display a constant stream of "1"
# When the EuroHiker's Gate IN LED is OFF, your terminal screen will display a constant stream of "0"
# Change the Gate's Pulse Rate so that you can see the changes from '0' to '1' and vice versa
# Note that the test script samples the Gate IN every 10ms or so
# this is so you can follow the 0/1/0 changes with your eyes! (the actual sample rate is a lot higher)
# Press Ctrl+z to stop the program
```

### GATE IN/OUT | OUT

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

Connect the Gate OUT of the EuroHiker module to your analog instrument's Gate IN.<br>
You could have it trigger an Envelope/ADSR for example.<br>

From the command prompt, enter:
```
cd /opt/unihiker/examples/100-EuroHiker/GATE_OUT
python Gate_Out_High_Low.py
# Watch your terminal window; it should read "low (0V)" & "High (5V)" repeatedly
# Also, look at the EuroHiker's Gate OUT LED - this should blink ON and OFF
# As the Gate OUT switches between High and Low, so should your gear react accordingly
# Press Ctrl+z to stop the program
```

### CV IN/OUT | IN

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

Connect the CV OUT of your analog instrument (LFO) to the CV IN of the EuroHiker Module.<br>
The brightness of the CV IN LED of the EuroHiker module should now run in sync with the CV OUT LED of your instrument. Set the LFO rate nice and slow - so we can read the changes better.<br>
Note that the brightness of LEDs can come across as a hard ON/OFF, but from the test script we'll see that the EuroHiker does measure a wide input range.

From the command prompt, enter:
```
cd /opt/unihiker/examples/100-EuroHiker/CV_IN
python CV_In_TEST.py
# The measured CV IN level is now shown in your teminal window as "P1 = xxxx"
# The value runs from 0 to 4095 (12-bit ADC)
# Note that the value is hardly ever exact 0 - this is becasue of the ADC's noise floor
# Press Ctrl+z to stop the program
```

### CV IN/OUT | OUT

Use PuTTY, or similar software, to SSH into the EuroHiker. The default username/Password:<br>
Username: <strong>root</strong><br>
Password: <strong>dfrobot</strong>

Connect the CV IN of your analog instrument (Oscillator's CV for example) to the CV OUT of the EuroHiker Module.<br>

CV OUT is a little bit special, because the 12-bit Digital-to-Analog Converter (DAC), a MCP4725, has an integrated EEPROM/Memory, which allows to set a boot-up output level.<br><br>
When you finished the built of the EuroHiker module, the CV OUT LED has been ON on every power up - this is simply the factory default. We can, and will, change this next. 

From the command prompt, enter:
```
cd /opt/unihiker/examples/100-EuroHiker/CV_OUT
python 1_i2c_scan.py
# This make take a little while.
# You should see a bunch of lines. What matters is that one of those lines reads: "Address of I2C device = 0x61"
# The CV OUT LED may also have switched off. It does not always happen - but it's ok - just carry on.
# You may have to retry this step until you see the address mentioned.
# It's worth pointing out that the MCP4725 comes in different flavors - address-wise that is.
# If this step returns a different address, you will need to edit the .py files mentioned in the next steps
# and replace 0x61 for the address you obtained. 

python 3_i2c_Set_DAC_Output_Level_at_Startup.py
# Wait for the "All right. PinPong go..." message to appear
# Press Ctrl+ z
# This should now have set CV OUT to zero at power-up.
# Switch the EuroHiker module OFF and ON again.
# The CV OUT LED should now be OFF at power up - and every power up from now on (unless you change it back of course)

# Log in again
cd /opt/unihiker/examples/100-EuroHiker/CV_OUT
python CV_Out_Random_Levels_16_Steps__Encoder_is_Rate.py
# Watch the CV OUT LED - its brightness changes through a 16 steps loop.
# Press the Rotary Encoder until you see another set of 16 values.
# Now it runs through these 16 steps of Brightness - and, of course, it outputs
# a control voltage level represented by the LED's brightness driving your Analog gear!
# Press Ctrl+z to stop the program
# The CV OUT LED will remain at the level before stopping the program until you restart the program
# or reboot the EuroHiker module.
```
<a id="supercollider"></a>
# SuperCollider (audio synthesis)
The EuroHiker's UniHiker board doesn't have Audio In/Out, but with an USB-A Audio Adapter it will be able to produce sound.<br><br>
I intend to redesign the PCBs so that the EuroHiker module either contains the audio adapter itself, or it interfaces with a separate audio module.<br><br>
I recommend you install the SuperCollider open source software. It enables the creation of wonderful sounds!<br><br>
Please visit my [step-by-step instructions](https://github.com/ErikOostveen/SuperColliderOnUniHiker) here on GitHub.
<hr>


