# Windows Unlock with RFID
I am using an RFID sensor and an arduino to unlock a Windows based device using keystrokes. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aryan | Greenwich High School | Electrical Engineering / Computer Science | Incoming Senior

<br/>

Myself             |  My Project
:-------------------------:|:-------------------------:
<img src="[https://github.com/AryanWadhwa05/Aryan-BSE-Portfolio/blob/gh-pages/squirrelssample.JPG?raw=true](https://github.com/AryanWadhwa05/Aryan-RFID-Windows-Unlocker/blob/f49b7dfcb4d26d832665ac643f16ba0fa34265b1/1.JPG)" width="400" height="250"/>  |  <img src= "https://github.com/AryanWadhwa05/Aryan-BSE-Portfolio/blob/gh-pages/Capture.JPG?raw=true" width="400" height="250" />

<br/>

# Reflection

Throughout my 3 weeks at Bluestamp Engineering, I have learned a great deal in both engineering and coding. I have been taught how to troubleshoot by myself, how to solder sadely, and how electrical components work. At this summer program, I felt more independent since we were informed by the instructors that they would not provide answers to the students questions unless we have tried at least three different ways to try to solve the problem. I think that Bluestamp’s way of teaching is very unique and promotes students to grasp the art of troubleshooting.

I discovered that both the software and Arduino aspects of my project were extremely enjoyable to do. From constantly debugging code to setting up my Arduino uno/micro, Bluestamp Engineering along with the amazing instructors were able to teach me a great deal through my 3 weeks at the program.

# Demo Night Video
This is my demonstration video that was recorded and presented on 7/21/2022. I run through what my project is about, how it works, and what it really does.

# Third Milestone/Modifications

<iframe src="https://youtu.be/W8EPWavnwPo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# Second Milestone

In my second milestone, I showed how I switched from an arduino uno to an arduino micro. Since the uno uses an ATmega328P chip, it doesn't have the capabilities to act as an HID and so is unable to send keystroke commands to the computer. The Arduino Micro uses an ATMEGA32u4 so it is able to act as both a keyboard and a mouse meaning i could send keystrokes to my computer such as WIN + L to lock the computer or my password to unlock the computer. Changing to the micro was very tedious as I had never worked with ICSP pins before and didn't know where they were or how they worked. Additionally, the code for the micro was slightly different as I had used code from the internet but it was buggy so I had to add more "if" statements to make sure the micro had a stable connection witht he RFID sensor.

<iframe src="https://youtu.be/DaXj_zLngkA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


# First Milestone

My first milestone was setting up and hooking up the RFID sensor with an Arduino Uno. The RFID RC522 requires 7 different connection including a GND and a 3V connection. You can't use a 5V connection as that overheats the sensor and this piece of equipment is genrally very sensitive to extra voltage. We then have a MISO, MOSI, SDA, SCK, and RST connections that all ensure the RFID is able to relay the information to the arduino and that the Uno is able relay the code to the RFID. MOSI makes sure that the sensor is able to recieve data from the host computer while MISO does the opposite. RST is a fail safe to make sure that voltage is correct and is kind of the middle man to make sure everything is going smoothly. SDA connects the RFID to the computer and makes connections possible and lastly SCK makes sure connections have a time limit and arrive on time.

<iframe src="https://youtu.be/YZ3usDSlLOQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
