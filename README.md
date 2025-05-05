# ece40862-lab-4--http-web-server-and-client-using-esp32-solved
**TO GET THIS SOLUTION VISIT:** [ECE40862 Lab 4 –HTTP Web Server and Client using ESP32 Solved](https://www.ankitcodinghub.com/product/ece40862-lab-4-http-web-server-and-client-using-esp32-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;94443&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECE40862 Lab 4 –HTTP Web Server and Client using ESP32 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column"></div>
</div>
<div class="layoutArea">
<div class="column">
1. Overview

The goal of this assignment is to familiarize you with Internet of Things (IoT). The IoT is a network of ‘smart’ embedded devices that connect and communicate via the Internet. The key to IoT is the interconnectivity of devices, which collect and exchange information through embedded software, cameras, and sensors which sense things like light, sound, distance, movement, temperature, and other environmental parameters. Smart embedded devices either operate autonomously or are controlled and monitored remotely. In this assignment, you will be using your ESP32 as a ‘smart’ embedded device operating automatically as well as communicating with the Internet.

The assignment is subdivided into two sections. In both sections, you will be implementing client-server communication using socket APIs and HTTP protocol. To review, network socket APIs are used to transfer messages between two software processes over a network. HTTP is an application layer protocol that defines different parameters of these messages, viz., type, format, length, authentication, error handling, etc.

1.1. Device as Client

A typical IoT system has a cloud server and multiple client devices.

Data flows from the IoT-devices to the cloud-server, as shown in this

image. In the first section, you will configure the ESP32 as an HTTP

client, measure the onboard temperature sensor data and hall sensor data, and SEND them periodically to an IoT Application Platform hosted on the internet. Specifically, you will be using the ThingSpeak IoT Platform as the server, collecting sensor data transmitted by the ESP.

1.2. Device as Server

In some scenarios/configuration, e.g., when you have a single IoT device and a local PC or a phone, the IoT device can also be setup as the server. In the second section of the assignment, you will configure the ESP32 as a HTTP web server, measure the onboard temperature

</div>
</div>
<div class="layoutArea">
<div class="column">
1 | P a g e

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
sensor data and hall sensor data, monitor the status of different GPIO pins, and SEND these data to the client ONLY WHEN THE CLIENT REQUESTS. You will be using your local PC or phone’s web browser (e.g., Chrome, Firefox, etc.) as the client. Additionally, you will also RECEIVE inputs from the client (i.e., the web browser) and control GPIO pins on the board based on these inputs.

NOTE: ESP as client (1.1) only SENDS data to cloud server. ESP as server (1.2) both SENDS data to client and RECEIVES data from client.

2. Programming Exercises 2.1. Hardware Interfacing

Interface the following components to the board (you’ve done this step many times now, so this should be super simple by now!)

• Two external LEDs (red and green) as GPIO outputs.

2.2. Software Implementation – ESP32 HTTP Client 2.2.1. Setup ThingSpeak

ThingSpeak is a free IoT Platform for gathering, analyzing, and visualizing data from IoT devices. ThingSpeak allows you to publish your sensor readings to their website and display them in a plot with time stamps. It provides a RESTful API for IoT devices (don’t worry if you don’t know what that means, it’s not important for this lab). You need to perform the following steps to configure it as your cloud server before you can start sending data from the ESP32.

<ul>
<li>Create a free account on the ThingSpeak website.</li>
<li>Create a new channel and enable two fields to receive data from the ESP32.
o Field1: Temperature Sensor o Field2: Hall Sensor

You’ll get an API key for posting data to your channel. This API key should be used for sending data to ThingSpeak from your ESP32.
</li>
</ul>
2.2.2. ESP32 Program (espclient.py)

Implement the following functionalities in your program.

• Connect to Internet and print out the local IP address (same as Lab 3).

• Initialize a hardware timer with a period of 16 seconds. Perform the following

operations:

o Measure the onboard temperature sensor data and hall sensor data.

o Display both the measured data on the terminal.

o SEND these data to ThingSpeak cloud server using socket API and HTTP

GET request. You need to use your specific Write API Key to upload data to

your channel in your ThingSpeak account. • Run your program for 5 minutes.

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
2.2.3. Sample Result

Your ThingSpeak account should show the visualizations for both sensor data, as shown in Fig. 1. Since, the timer fires every 16 seconds, a maximum of 18 data points (for each sensor) will be uploaded by your client over a duration of 5 minutes. Fig. 1 only shows a sample screenshot from the ThingSpeak website showing only 4 data points. Run your program for 5 minutes. After the program has finished, take a screenshot (similar to Fig. 1) from the ThingSpeak website showing ~18 data points.

Figure 1. Screenshot from ThingSpeak showing Temperature and Hall Senor data

2.3. Software Implementation – ESP32 HTTP Server 2.3.1. ESP32 Program (espserver.py)

Implement the following functionalities in your program. You can update the espserver.py file which has been provided to you.

<ul>
<li>Connect to Internet and print out the local IP address (same as Lab 3 Section 2.2.1).</li>
<li>Measure the onboard temperature sensor data and hall sensor data.</li>
<li>Measure the values of different GPIO pins, viz., two LEDs.</li>
<li>Use the function web_page (present in the provided file) to create simple HTML text
to build the webpage with 2 sensor data and 2 LED pin values. The HTML text has been provided in the espserver.py. You can use the 4 variables defined in the file (temp, hall, red_led_state, green_led_state) to measure the sensor and pin values.
</li>
<li>Create an HTTP server using socket API to listen for incoming requests from any client (browser on your local PC or phone connected to same Wi-Fi network).</li>
<li>Use an infinite loop: Whenever your ESP server receives any client request (e.g., pressing any button on the webpage), it should use the function web_page to update the HTML text with the current sensor and LED pin values, SEND necessary HTTP headers and finally SEND the updated HTML text as the response to the client.</li>
</ul>
</div>
</div>
<div class="layoutArea"></div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
2.3.2. Sample Result

Open a web browser on your PC or phone and type in the IP Address of your ESP32 server. You should be able to access the web page with the latest sensor readings and GPIO states.

NOTE: Pressing any buttons on the webpage counts as one CLIENT REQUEST. So, every time you press any button, the temperature, hall, and led states should update. e.g., if you press the RED ON button, red led connected to your board should light up, and the RED LED Current State should display ON as shown in Fig. 2. Now if you press the GREEN ON button, green led connected to your board should light up, and the GREEN LED Current State should display ON, as shown in Fig. 3.

Figure 2. Webpage on pressing RED ON button

Figure 3. Webpage on pressing GREEN ON button

</div>
</div>
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
</div>
