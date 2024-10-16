<h1>Web-Controlled Smart Home System</h1>

<img src="https://imgur.com/CJsOHkw.png"  height="80%" width="80%" alt="landing page"/> 

<h2>Description</h2>
Iot based home automation system is built using a group of sensors connected through
Arduino Uno with its input/output pins. These devices are connected with local Wi-Fi using a
communicating module called esp8266-01. Different application such as turning ON and
OFF lights either manually or ,detecting the gaz leak and warn the owner ,giving
informations about the ambient temperature and switch on and off some AC devices like fan,
intrusion detection, access using RFID, and license plate detection.


<h2>Languages, Frameworks and Utilities Used</h2>
- <b>React Js</b>
- <b>FireBase</b> 
- <b>Python</b>
- <b>YOLO</b>
- <b>OCR (Optical Character Recognition)</b>

<h2>Project Requirement</h2>
<h3>Sensors</h3>
-<b>MQ2 Gas Sensor<b>
-<b>DHT-11 Sensor</b>
-<b>PIR Motion Sensor </b>
  <h3>Controllers</h3>
-<b>Arduino UNO</b>
-<b>Esp 8266 WIFI module</b>
  <h3>Other Hardwares </h3>
-<b>RC522 RFID</b>
-<b>SG90 Servo motor</b>
-<b>Leds and a buzzers</b>

<h2>Protocols Used</h2>
-Analogue Output 
-Wire Protocol 
-Digital Output
-Wi-Fi, HTTP/MQTT
-Serial (UART)

<h2>Features</h2>
- lighting Control From the Website <br>
- Get notification and turn the buzzer on in Case of any alert <br>
<img src="https://imgur.com/kMsEtai.png"  height="80%" width="80%" alt="alert"/> <br>
<h3>Kitchen </h3>
- Montior the gaz level <br> <br>
<img src="https://imgur.com/fx6L7gy.png"  height="80%" width="80%" alt="Kitchen"/> <br>
<h3>Living Room</h3>
- Monitor the temperature and the humidity <br>
- Turn the Fan automaticaly if the temperature passed the threashold <br> <br>
<img src="https://imgur.com/O3KiCaf.png"  height="80%" width="80%" alt="living Room"/> 
<br><br>
- The abitility to change the threashold wanted to start turning the fan <br>
<img src="https://imgur.com/v0xORdW.png"  height="80%" width="80%" alt="temperature"/> 
<br>

<h3>Door Access</h3>
- Using the RFID reader to scan the RFID Tag and compare it to te databse of authenticated Tags in Firebase
<img src="https://imgur.com/bgneKHX.png"  height="80%" width="80%" alt="temperature"/> 
<br>

<h3>Garage Access</h3>
- The YOLO (You Only Look Once) algorithm is used for Automatic License Plate Detection. YOLO is a real-time object detection system that processes images in a single pass, dividing the image into a grid. Each grid cell predicts bounding boxes for potential objects and their corresponding confidence scores.<br>
- For License Plate Recognition (ANPR/ALPR), the steps are:
    1-Image Input: Capture an image or video frame containing a vehicle.<br>
    2-License Plate Detection: Using YOLO, the license plate is detected by predicting bounding boxes.<br>
    3-Character Extraction: After localizing the license plate, the characters on it are extracted.<br>
    4-OCR (Optical Character Recognition): An OCR tool like Tesseract is used to recognize the characters and convert them into text.<br><br>

- To implement this, the model is trained using PyTorch, leveraging datasets of annotated license plate images. Once trained, OpenCV is used to process images, detect the license plates, and the OCR extracts the text. Post-processing enhances accuracy, making it suitable for real-world applications like toll gate operations or vehicle tracking.<br>

