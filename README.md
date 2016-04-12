# mini-IoT
This experiment showcases a miniature version of the Internet of Things. 

An Arduino UNO board and an Android device is used in this experiment. The android app communicates with the arduino wirelessly and turns on and off Light, Fan and Sound devices connected to the arduino. The Light,Fan and Sound devices are connected to the arduino via breadboard and wires respectively. The arduino receives power from the USB cable. PHP language is used to pass messages to the arduino using the serial com port of the PC via the USB cable.

The goal of this experiment is to demonstrate the flexibility and power of the android operating system when used together with the arduino UNO board. This experiment proves that anyone with basic programming skills can create something very useful.

<b>Instructions to make the project up and running:</b>

1. Open the Arduino code in the Arduino folder into your Arduino IDE and upload it to the Arduino UNO board.
2. In the Arduino IDE check the COM port of your Arduino and update it in "device.php" file in the php folder.
2. Upload the php files in the php folder to your XAMPP server in "htdocs/your_folder_name" and start the server(Apache and MySQL).
3. Download the Android project from the "android" folder and open it into Android Studio IDE.
4. In ActivityMain replace the IP Address "192.168.0.105" by your machines local IP address.
5. In ActivityMain replace the path "/arduino/test/device.php?name=" by your php file path inside htdocs. For example "/my_folder/device.php?name=".
6. Keep Arduino UNO board connected to the same PC with your XAMPP server running.
7. Run the android project in your android device(I haven't tested in the emulator but i think it should work fine. Use Android 4.1 and above).
8. Connect your Android device via WiFi in the same network as your Laptop/PC.
9. Run and test the app. When clicked on a particular card it should turn the devices on and off(Check Android monitor for Logcat message from the server and for any other error).
