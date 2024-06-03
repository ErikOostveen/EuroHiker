# EuroHiker

The EuroHiker module is designed to provide a programmable platform capable of executing various functions, fitting seamlessly into the world of EuroRack where modules are typically fine-tuned to excel in their designated tasks.

![EuroHiker_With_Exp_Cable](https://github.com/ErikOostveen/EuroHiker/assets/40121318/e78d3542-780f-490a-b9b9-739aca90ba37)

The EuroHiker module is based on the popular (Linux) Unihiker single board computer by [DFRobot](https://www.dfrobot.com/product-2691.html)

The UniHiker board comes standard with WiFi/Bluetooth, Light Sensor, Microphone, Accelerometer sensor, Gyroscope sensor, Buzzer, MicroSD card slot and Various I/O connectivity (PWM, ADC, I2C, UART, USB, SPI)

The EuroHiker module adds to this already impressive list of features MIDI IN/OUT, Gate IN/OUT, Control Voltage IN/OUT, two push buttons, a Rotary Encoder with built in Red/Green/Blue LEDs plus another push button. The module also has an ON/OFF switch - and last but not least, offers an expansion interface (26pins) for you to experiment and interact with the EuroHiker module through your own desgins!

Download the [EuroHiker Visual Summary (PDF | 19Mb) here](https://github.com/ErikOostveen/EuroHiker/files/15461125/EuroHiker_OnePager.pdf)

Module Specs
<br>• 3U/20HP = approx. H128mm x W101mm
<br>• Depth approx. 40mm
<br>• +12V = 600mA, -12V = 25mA, +5V = 0mA

The EuroHiker module is designed to provide a programmable platform capable of executing various functions, fitting seamlessly into the world of EuroRack where modules are typically fine-tuned to excel in their designated tasks.

The EuroHiker module, on the other hand, empowers you to navigate through folders containing Python programs, each leveraging the module's extensive feature set.

The idea is to have the flexibility to explore numerous concepts, allowing you to test them before deciding whether to further develop them using another development board or to retain them with

# Let's Assemble! - EuroHiker PCB 1 of 2

The first part, of two, in assembling the EuroHiker module, is to gather all required components. I had the PCB, which houses the front panel's components, partially populated becasue I had some of the parts in stock. See overview below:

![pcb_1_overview](https://github.com/ErikOostveen/EuroHiker/assets/40121318/3e42fe15-b6ab-46be-93e7-86d1de6bcb39)

### A
Partially populated PCB. 
What follows are the suggested steps to building the EuroHiker module. I have also included links to some of the components - these are suggestions also. Sometimes links come back "blocked"; in that case just copy/paste the link into your browser.   

### B
Start with the Edge Connector (BBC micro:bit).<br>
Link: https://kitronik.co.uk/products/4148-edge-connector-header-for-bbc-microbit<br>
![big_connector2](https://github.com/ErikOostveen/EuroHiker/assets/40121318/a196fd32-167f-4dd2-93af-0fca1281fff7)

### C
Solder the 2 Right-Angled 2Pin Sockets.<br> 
Link:https://www.lcsc.com/product-detail/Female-Headers_CONNFLY-Elec-DS1024-1x2R2_C7509534.htmld<br>
These sockes are not mandatory; you can solder wires directly from this PCB to the USB breakout boards (mentioned further down in the steps).<br>
![sockets](https://github.com/ErikOostveen/EuroHiker/assets/40121318/1c3608f7-a3e0-456e-986a-cee843d94a3a)

### D
Solder the 6 3.5mm jack sockets. Keep in mind; the 2 MIDI sockets are STEREO sockets (Green on image) the remaining 4 are MONO (Black on the image).
By far the best place to get these jack sockets is THONK.<br>
Link: https://www.thonk.co.uk/shop/3-5mm-jacks/<br>
![JACKS](https://github.com/ErikOostveen/EuroHiker/assets/40121318/659e82f4-a1bd-4916-b729-4ecb5da68780)

### E & F
The tallest components go last (we'll get to the LEDs later); "E" first:<br>
1 x Miniature Toggle (the Power) Switch<br>
Link: https://www.digikey.co.uk/en/products/detail/e-switch/100SP1T1B4M2QE/378824?s=N4IgTCBcDaIIwAYEGUAKcAqcBCAWAsmAIoCiIAugL5A<br>
2 x Push Buttons (Left/Right) (6.2x6.2x13mm)<br>
Link: https://www.lcsc.com/product-detail/Tactile-Switches_Diptronics-DTS-66K-V_C141877.html
Then "F":<br>
Link: 1 x Rotary RGB Encoder<br>
https://uk.robotshop.com/products/rotary-rgb-encoder-illuminated
![toggle_sw_buttons_encoder](https://github.com/ErikOostveen/EuroHiker/assets/40121318/ffab539d-409b-4091-8817-ebc3274af27b)












