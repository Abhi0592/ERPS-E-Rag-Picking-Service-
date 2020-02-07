# ERPS
DEVELOPMENT OF SMART DUMPYARD &WASTE MONITORING SYSTEM

A PROJECT REPORT

In partial fulfillment for the award of the degree

Of

BACHELOR OF ENGINEERING

 
Under the guidance of                                                          Submitted by 
Dr. Dilip Kumar(Professor)                                     Gunjan Gupta(GCS/SL/15/4016)
Dr. Surinder Singh(Professor)                                    Kumari Beena Singh(1730981)      ECE Department                                                                        Ritika Negi(1640015)
                                                                                               Ishpreet Kaur(1640092)
                                                                                                 Anjali Singh(1730982)
                                                                                         Harshit Udainiya(1640048)
                                                                                                            Sahil(1740588)
                                                                                            Satish Kaushik(1740603) 
                                                                                           Kanha Jain(1740560)
                                                                              Abhishek Kumar Rai (1740592)



SANT LONGOWAL INSTITUTE OF ENGINEERING AND TECHNOLOGY,
LONGOWAL – 148106, DISTRICT- SANGRUR, PUNJAB, INDIA
AUGUST, 2019


TABLE OF CONTENTS

SR. NO.	TITLE	REMARKS
1.	Certificate	
2.	Acknowledgement	
3.	Abstract	
4.	Introduction	
5.	Problem statement	
6.	System design	
	6.1 Hardware requirements
6.1a Arduino Uno
6.1b JSN-SR04T
6.1c SIM900A
6.2 Software requirements
6.2a Arduino IDE
6.2b Firebase	
7.	Conclusion	
8.	Future enhancements	
9.	References	







CERTIFICATE
We hereby certify that the work which is being presented in the B.E. Project Report entitled “Development of smart dumpyard and waste monitoring system”, in partial fulfillment of the requirements for the award of the Bachelor of Engineering and submitted to the Department of Electronics & Communication Engineering of SLIET, Longowal is an authentic record of our own work carried out during a period from March 2019 to August 2019 under the supervision of Dr. Dilip Kumar (Professor) & Dr. Surinder Singh (Professor) ECE Department. 
	The matter presented in this report has not been submitted by us for the award of any other degree elsewhere.

                                                                                  			Signature of Candidate
		
This is to certify that the above statement made by the candidate is correct to the best of my knowledge.
								   Signature of Supervisor	
  Date: 	                                                                                      Dr. Dilip Kumar
                                                                                                                                     Dr. Surinder Singh
                                                                                                        Professor, ECE Department  		           
	
				
Head of Department
Electronics & Communication Engineering
SLIET, Longowal	
                                         			  




ACKNOWLEDGMENT

We would like to express our sincere gratitude to Dr. Dilip Kumar (Professor) & Dr. Surinder Singh (Professor) of the department of Electronics and Communication, whose role as project guide was invaluable for the project. We are extremely thankful for the keen interest he took in advising us, for the books and reference materials provided for the moral support extended to us.

Last but not the least we convey our gratitude to all the teachers for providing us the technical skill that will always remain as our asset and to all non-teaching staff for the gracious hospitality they offered us.


   
Place: SLIET, LONGOWAL

 Date:







Department of Electronics & Communication
SLIET, Longowal 
ABSTRACT

In the recent decades, Urbanization has increased tremendously. At the same phase there is an increase in waste production. Waste management has been a crucial issue to be considered. This paper is a way to achieve this good cause. In this project, smart dumpyard is built on a microcontroller based platform Arduino Uno board which is interfaced with GSM modem and Ultrasonic sensor. Ultrasonic sensor is placed in the dumpyard which will measure the status of the dumpyard. The threshold stature is set as 25cm. Arduino will be programmed in such a way that the real time monitoring of the garbage of dumpyard can be done. With the help of GSM we send the actual levels of garbage in dumpyard being recorded using ultrasonic sensors on cloud and fetch the recorded data on hand held mobile app on real time. According to the fetched data the necessary action and waste management takes place. At regular intervals dumpyard will be squashed. Once these smart dumpyards are implemented on a large scale, by replacing our traditional dumpyards present today, waste can be managed efficiently as it avoids unnecessary lumping of wastes on roadside. Foul smell from these rotten wastes that remain untreated for a long time, due to negligence of authorities and carelessness of public may lead to long term problems. Breeding of insects and mosquitoes can create nuisance around promoting unclean environment. This may even cause dreadful diseases.





























INTRODUCTION

We are living in an age where tasks and systems are fusing together with the power of IOT to have a more efficient system of working and to execute jobs quickly! With all the power at our finger tips this is what we have come up with.The Internet of Things (IoT) shall be able to incorporate transparently and seamlessly a large number of different systems, while providing data for millions of people to use and capitalize. Building a general architecture for the IoT is hence a very complex task, mainly because of the extremely large variety of devices, link layer technologies, and services that may be involved in such a system. One of the main concerns with our environment has been solid waste management which impacts the health and environment of our society. The detection, monitoring and management of wastes is one of the primary problems of the present era. The traditional way of manually monitoring the wastes in waste bins is a cumbersome process and utilizes more human effort, time and cost which can easily be avoided with our present technologies. This is our solution, a method in which waste management is automated. This is our IoT Garbage Monitoring system, an innovative way that will help to keep the cities clean and healthy.

























PROBLEM STATEMENT

We want to make world a cleaner place to live in. Due to rising air pollution it adversely causes
breathing problem for older people, pregnant women, and small kids. The major causes for air
pollution are automobiles, open disposal of garbage, factories and mills. So we came up with
innovative and efficient method for proper management of waste. Due to garbage, harmful gases
get evolved in environment and they attract harmful diseases towards we being. This problem
occurs when pile of garbage is not cleared or picked up timely which should be done instantly as
soon as garbage gets collected because the schedule for Municipal Corporation’s garbage truck is fixed. The issue occurs at the places of garbage bin which are kept in every block, street. This project combats the problem of overflowing solid waste bins which pollute the surroundings. The level of garbage present in any bin is determined by the ultrasonic distance measuring sensor. When the garbage level in any garbage bin exceeds a pre-defined level, then the microcontroller send an alert message to the e-monitoring station, the workstation then assigns the nearest garbage collecting truck to collect the garbage from such bins.


  

SYSTEM DESIGN

What our system does is it gives a real time indicator of the garbage level in a trashcan at any given time. Using that data we can then optimize waste collection routes and ultimately reduce fuel consumption. It allows trash collectors to plan their daily/weekly pick up schedule. An Ultrasonic Sensor is used for detecting whether the trash can is filled with garbage or not. Here Ultrasonic Sensor is installed at the top of Trash Can and will measure the distance of garbage from the top of Trash can and we can set a threshold value according to the size of trash can.  If the distance will be less than this threshold value, means that the Trash can is full of garbage and we will indicate it using red color in mobile application. 






















HARDWARE REQUIREMENTS
We will need the following hardware to accomplish our project. 
1. Arduino Uno.
2. JSN-SR04T ultrasonic sensor.
3. GSM module. 
4. Connecting wires. 
 
 ARDUINO UNO  
 Arduino is an open-source platform used for building electronics projects. Arduino consists of both a physical programmable circuit board (often referred to as a microcontroller) and a piece of software, or IDE (Integrated Development Environment) that runs on your computer, used to write and upload computer code to the physical board. • The Arduino platform has become quite popular with people just starting out with electronics, and for good reason. Unlike most previous programmable circuit boards, the Arduino does not need a separate piece of hardware (called a programmer) in order to load new code onto the board – you can simply use a USB cable. Additionally, the Arduino IDE uses a simplified version of C++, making it easier to learn to program. Finally, Arduino provides a standard form factor that breaks out the functions of the micro-controller into a more accessible package. The Arduino is a microcontroller board based on the ATmega8. It has 14 digital -input/output pins (of which 6 can be used as PWM outputs), 6 analog inputs, a16 MHz ceramic resonator, a USB connection, a power jack, an ICSP header, and a reset button. It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with a ACto-DC adapter or battery to get started .The Uno differs from all preceding boards in that it does not use the FTDI USB-to-serial driver chip. Instead, it features the Atmega16U2 (Atmega8U2 up to version R2) programmed as a USB-to-serial converter .Revision 2 of the Uno board has a resistor pulling the 8U2HWB line to ground, making it easier to put into DFU mode. Revision of the board has the following new features: • Pin out: added SDA and SCL pins that are near to the AREF pin and two other new pins placed near to the RESET pin, the IOREF that allow the shields to adapt to the voltage provided from the board. In future, shields will be compatible with both the board that uses the AVR, which operates with 5V and with the Arduino Due that operates with 3.3V. The second one is a not connected pin that is reserved for future purposes. • Stronger RESET circuit.  • AT mega 16U2 replace the 8U2.  "Uno" means one in Italian and is named to mark the upcoming release of Arduino 1.0. The Uno and version 1.0 will be the reference versions of Arduino, moving forward. The Uno is the latest in a series of USB Arduino boards, and the reference model for the Arduino platform. 
 
Figure 2: ARDUINO UNO BOARD

Pin Description
Pin Category	Pin Name	Details
Power	Vin, 3.3V, 5V, GND	Vin: Input voltage to Arduino when using an external power source.
5V: Regulated power supply used to power microcontroller and other components on the board.
3.3V: 3.3V supply generated by on-board voltage regulator. Maximum current draw is 50mA.
GND: ground pins.
Reset	Reset	Resets the microcontroller.
Analog Pins	A0 – A5	Used to provide analog input in the range of 0-5V
Input/Output Pins	Digital Pins 0 - 13	Can be used as input or output pins.
Serial	0(Rx), 1(Tx)	Used to receive and transmit TTL serial data.
External Interrupts	2, 3	To trigger an interrupt.

PWM	3, 5, 6, 9, 11	Provides 8-bit PWM output.
SPI	10 (SS), 11 (MOSI), 12 (MISO) and 13 (SCK)	Used for SPI communication.
Inbuilt LED	13	To turn on the inbuilt LED.
TWI	A4 (SDA), A5 (SCA)	Used for TWI communication.
AREF	AREF	To provide reference voltage for input voltage.
 
		





Arduino Uno Technical Specifications
Microcontroller	ATmega328P – 8 bit AVR family microcontroller

Operating Voltage	5V
Recommended Input Voltage	7-12V
Input Voltage Limits	6-20V
Analog Input Pins	6 (A0 – A5)
Digital I/O Pins	14 (Out of which 6 provide PWM output)
DC Current on I/O Pins	40 Ma
DC Current on 3.3V Pin	50 Ma
Flash Memory	32 KB (0.5 KB is used for Bootloader)
SRAM	2 KB
EEPROM	1 KB

JSN-SR04T ULTRASONIC SENSOR
The JSN-SR04T is an easy to use waterproof ultrasonic distance sensor with a range of 25 to 450 cm.
 The sensor comes with a 2.5 m long cable that connects to a breakout board which controls the sensor and does all the processing of the signal. Note that only the sensor and the cable itself are waterproof, if you get water onto the breakout board, the sensor might stop working.
An ultrasonic distance sensor works by sending out ultrasound waves. These ultrasound waves get reflected back by an object and the ultrasonic sensor detects them. By timing how much time passed between sending and receiving the sound waves, you can calculate the distance between the sensor and an object.
Distance (cm) = Speed of sound (cm/µs) × Time (µs) / 2
Where Time is the time between sending and receiving the sound waves in microseconds.
 
Figure 2: JSN-SR04T Ultrasonic Sensor 

JSN-SR04T Specifications

Operating voltage	5 V
Operating current	30 Ma
Quiescent current	5 Ma
F

Requency	40 kHz
Measuring range	25-450 cm
Resolution	2 mm
Measuring angle	45-75 degrees
Sensor dimensions	23.5 x 20 mm, 2.5 m long cable
PCB dimensions	41 x 28.5 mm
Mounting hole	18 mm









SIM900A GSM/GPRS MODULE

The SIM900 is a complete Quad-band GSM/GPRS solution in a SMT module which can be embedded in the customer applications.   Featuring an industry-standard interface, the SIM900 delivers GSM/GPRS 850/900/1800/1900MHz performance for voice, SMS, Data, and Fax in a small form factor and with low power consumption. With a tiny configuration of 24mm x 24mm x 3 mm, SIM900 can fit almost all the space requirements in your M2M application, especially for slim and compact demand of design. 
 
” SIM900 is designed with a very powerful single-chip processor integrating 
” Quad - band GSM/GPRS module with a size of 24mmx24mmx3mm 
” SMT type suit for customer application 
” An embedded Powerful TCP/IP protocol stack 
” Based upon mature and field-proven platform, backed up by our support 
   service, from definition to design and production

GENERAL FEATURES
” Quad-Band 850/ 900/ 1800/ 1900 MHz
 ” GPRS multi-slot class 10/8
 ” GPRS mobile station class B
 ” Compliant to GSM phase 2/2+ – Class 4 (2 W @850/ 900 MHz) – Class 1 (1W @ 1800/1900MHz) 
” Dimensions: 24* 24 * 3 mm
 ” Weight: 3.4g
 ” Control via AT commands (GSM 07.07 ,07.05 and SIMCOM enhanced AT Commands)
 ” SIM application toolkit
 ” Supply voltage range 3.4 ... 4.5 V 
” Low power consumption 
” Operation temperature: -30 °C to +80 °C



 INTERFACES
” Interface to external SIM 3V/ 1.8V 
” analog audio interface ” RTC backup
 ” SPI interface ” Serial interface 
” Antenna pad ” I2C ” GPIO ” PWM ” ADC 
                     
  COMPATIBILITY
” AT cellular command interface

 
Figure 4: SIM900A GSM/GPRS MODULE





CIRCUIT DIAGRAM
 










SOFTWARE REQUIREMENTS
    
•	Arduino IDE
•	Text Editor
•	Android Application
•	Firebase

ARDUINO IDE
The open-source Arduino Software (IDE) makes it easy to write code and upload it to the board. It runs on Windows, Mac OS X, and Linux. The environment is written in Java and based on Processing and other open-source software. This software can be used with any Arduino board. The Arduino development environment contains a text editor for writing code, a message area, a text console, a toolbar with buttons for common functions, and a series of menus. It connects to the Arduino hardware to upload programs and communicate with them.Software written using Arduino are called sketches. These sketches are written in thetext editor. Sketches are saved with the file extension .ino. It has features for cutting/pastingand for searching/replacing text. The message area gives feedback while saving and exportingand also displays errors. The console displays text output by the Arduino environmentincluding complete error messages and other information. The bottom right-hand corner ofthe window displays the current board and serial port. The toolbar buttons allow you to verifyand upload programs, create, open, and save sketches, and open the serial monitor.











ANDROID APPLICATION
 
Figure 5: HOME PAGE OF APPLICATION

 
Figure 6: GETTING THE LOCATION

 
Figure 7: GARBAGE LEVEL


FIREBASE
Firebase is a mobile-backend-as-a-service that provides powerful features for building mobile apps. Firebase has three core services: a realtime database, user authentication and hosting.

FIREBASE SERVICES
 
Firebase Services can be divided into two groups:
Develop & test your app
•	Realtime Database
•	Auth
•	Test Lab
•	Crashlytics
•	Cloud Functions
•	Firestore
•	Cloud Storage
•	Performance Monitoring
•	Crash Reporting
•	Hosting

Grow & Engage your audience
•	Firebase Analytics
•	Invites
•	Cloud Messaging
•	Predictions
•	AdMob
•	Dynamic Links
•	Adwords
•	Remote Config
•	App Indexing

PROGRAMS

1.	Arduino code for sending data to cloud
 #include <SoftwareSerial.h>
/* Create object named SIM900 of the class SoftwareSerial */
SoftwareSerial SIM900(5, 6);
const int trigPin1 = 7;
const int echoPin1 = 8;

long duration,distance,sensor1;
void setup()
{
  delay(10000);
pinMode(trigPin1, OUTPUT);
pinMode(echoPin1, INPUT);
delay(10000);
  SIM900.begin(9600);  /* Define baud rate for software serial communication */
  Serial.begin(9600); /* Define baud rate for serial communication */
}
void loop() {
  Serial.println("TCP Receive :");
  Serial.print("AT\\r\\n");
  SIM900.println("AT"); /* Check Communication */
  delay(1000);
  ShowSerialData(); /* Print response on the serial monitor */
  delay(1000);
  Serial.print("AT+CIPMODE=0\\r\\n"); 
  SIM900.println("AT+CIPMODE=0"); /* Non-Transparent (normal) mode for TCP/IP application */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CIPMUX=0\\r\\n");
  SIM900.println("AT+CIPMUX=0");  /* Single TCP/IP connection mode */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CGATT=1\\r\\n");
  SIM900.println("AT+CGATT=1"); /* Attach to GPRS Service */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CREG?\\r\\n");
  SIM900.println("AT+CREG?"); /* Network registration status */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CGATT?\\r\\n");
  SIM900.println("AT+CGATT?");  /* Attached to or detached from GPRS service */ 
  delay(1000); 
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CSTT=\"BSNLNET\",\"\",\"\"\\r\\n");
  SIM900.println("AT+CSTT=\"BSNLNET\",\"\",\"\""); /* Start task and set APN */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CIICR\\r\\n");
  SIM900.println("AT+CIICR"); /* Bring up wireless connection with GPRS */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CIFSR\\r\\n");
  SIM900.println("AT+CIFSR"); /* Get local IP address */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CIPSTART=\"TCP\",\"api.thingspeak.com\",\"80\"\\r\\n");
  SIM900.println("AT+CIPSTART=\"TCP\",\"api.thingspeak.com\",\"80\"");  /* Start up TCP connection */
  delay(1000);
  ShowSerialData();
  delay(1000);
  Serial.print("AT+CIPSEND\\r\\n");
  SIM900.println("AT+CIPSEND"); /* Send data through TCP connection */
  delay(800);
  ShowSerialData();
  delay(1000);
  SonarSensor(trigPin1, echoPin1);
  sensor1 = distance;
 
  Serial.println(sensor1);
 
  ShowSerialData();
  delay(1000);
  if(sensor1<30)
  {
   Serial.print("GET /update?api_key=I2HRCP3BRFUOVDZD&field1=70\\r\\n");
   SIM900.print("GET /update?api_key=I2HRCP3BRFUOVDZD&field1=70\r\n\x1A");  /* URL for data to be sent to */ /*DUSTBIN IS fUll*/ /*RED*/
   delay(1000);
   ShowSerialData();
   delay(1000);
   } 
   if(sensor1<40&&sensor1>30)
  {
   Serial.print("GET /update?api_key=I2HRCP3BRFUOVDZD&field1=40\\r\\n");
   SIM900.print("GET /update?api_key=I2HRCP3BRFUOVDZD&field1=40\r\n\x1A");  /* URL for data to be sent to */ /*DUSTBIN IS HALF FILLED*/ /*RED*/
   delay(1000);
   ShowSerialData();
   delay(1000);
   } 
  if(sensor1>40)
  {
  Serial.print("GET /update?api_key=I2HRCP3BRFUOVDZD&field1=10\\r\\n");
  SIM900.print("GET /update?api_key=I2HRCP3BRFUOVDZD&field1=10\r\n\x1A");  /* URL for data to be sent to */ /*DUSTBIN IS EMPTY*/ /*GREEN*/
  delay(1000);
  ShowSerialData();
  delay(1000);
  }
  Serial.print("AT+CIPSHUT\\r\\n");
  SIM900.println("AT+CIPSHUT"); /* Deactivate GPRS PDP content */
  delay(1000);
  ShowSerialData();
  delay(1000);
}

void ShowSerialData()
{
  while(SIM900.available()!=0)  /* If data is available on serial port */
  Serial.write(char (SIM900.read())); /* Print character received on to the serial monitor */
}
void SonarSensor(int trigPin,int echoPin)
{
digitalWrite(trigPin, LOW);
delay(100);
digitalWrite(trigPin, HIGH);
delay(500);
digitalWrite(trigPin, LOW);
duration = pulseIn(echoPin, HIGH);
distance = (duration/2) / 29.1;
 }



2.	Software Code
 package com.example.java.ewms;

import android.content.Intent;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.Window;
import android.view.WindowManager;

public class SplashActivity extends AppCompatActivity {
    private int SLEEP_TIMER=3;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);


        requestWindowFeature(Window.FEATURE_NO_TITLE);
        getWindow().setFlags(WindowManager.LayoutParams.FLAG_FULLSCREEN, WindowManager.LayoutParams.FLAG_FULLSCREEN);
        setContentView(R.layout.activity_splash);
       // getSupportActionBar().hide();
        LogoLauncher logoLauncher=new LogoLauncher();
        logoLauncher.start();
    }

        private class LogoLauncher extends Thread{
            public void run (){
                try {
                    sleep(1000*SLEEP_TIMER);
                }catch (InterruptedException e){
                    e.printStackTrace();
                }
                Intent intent = new Intent(SplashActivity.this,MainActivity.class);
                startActivity(intent);
                SplashActivity.this.finish();

            }
        }



    }

3.	Software Code
 package com.example.java.ewms;

import android.Manifest;
import android.app.ProgressDialog;
import android.content.DialogInterface;
import android.content.Intent;
import android.content.pm.PackageManager;
import android.location.LocationManager;
import android.os.Handler;
import android.support.annotation.NonNull;
import android.support.v4.app.ActivityCompat;
import android.support.v4.content.ContextCompat;
import android.support.v7.app.AlertDialog;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;

import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.auth.AuthResult;
import com.google.firebase.auth.FirebaseAuth;
import com.google.firebase.auth.FirebaseUser;

public class MainActivity extends AppCompatActivity {
    private EditText Name;
    private EditText Password;
    private TextView Info;
    private Button Login;
    private int LOCATION_REQUREST_CODE =1;
private int counter=5;
private TextView userRegistration;
private FirebaseAuth firebaseAuth;
    LocationManager lm;
private ProgressDialog progressDialog;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Name=(EditText)findViewById(R.id.etName);
        Password=(EditText)findViewById(R.id.etPassword);
        Info=(TextView)findViewById(R.id.tvInfo);
        Login=(Button)findViewById(R.id.btnLogin);
        userRegistration=(TextView)findViewById(R.id.tvRegister);

         lm = (LocationManager) getSystemService(LOCATION_SERVICE);


        if(ContextCompat.checkSelfPermission(MainActivity.this,
                Manifest.permission.ACCESS_FINE_LOCATION)==PackageManager.PERMISSION_GRANTED){
            Toast.makeText(MainActivity.this,"you have already granted the location access permission",Toast.LENGTH_LONG).show();
            boolean enabled = lm.isProviderEnabled(LocationManager.GPS_PROVIDER);
            if(!enabled) {
                showDialogGPS();
            }
            }
            else{
            requestLocationPermission();

        }

        Info.setText("No of attempts remaining:5");
        firebaseAuth=FirebaseAuth.getInstance() ;
        progressDialog=new ProgressDialog(this);
        FirebaseUser user = firebaseAuth.getCurrentUser();
        if(user!=null){
            finish();
            startActivity(new Intent(MainActivity.this,Maps1Activity.class));
        }
        Login.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                if(Name.getText().toString().equals(null) || Password.getText().toString().equals(null)){
                    Toast.makeText(MainActivity.this, "field can't be empty", Toast.LENGTH_SHORT).show();
                    return;}
                validate(Name.getText().toString(),Password.getText().toString());

            }
        });
        userRegistration.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                startActivity (new Intent (MainActivity.this,RegistrationActivity.class));
            }
        });

    }
    private void validate(String userName, String userPassword){
        progressDialog.setMessage("Please Wait for a Moment");
        progressDialog.show();

        firebaseAuth.signInWithEmailAndPassword(userName,userPassword).addOnCompleteListener(new OnCompleteListener<AuthResult>() {
            @Override
            public void onComplete(@NonNull Task<AuthResult> task) {
           if(task.isSuccessful()){
               progressDialog.dismiss();
               Toast.makeText(MainActivity.this, "Login Successful", Toast.LENGTH_SHORT).show();
               startActivity(new Intent(MainActivity.this,Maps1Activity.class));

           }else{
               Toast.makeText(MainActivity.this, "Login Failed", Toast.LENGTH_SHORT).show();
               counter--;
               Info.setText("No of attempts remaining:"+ counter);
               progressDialog.dismiss();
               if(counter==0){
                   Login.setEnabled(false);
               }
           }
            }
        });
    }
    private void showDialogGPS() {
        AlertDialog.Builder builder = new AlertDialog.Builder(this);
        builder.setCancelable(false);
        builder.setTitle("Enable GPS");
        builder.setMessage("Please enable GPS");
        builder.setInverseBackgroundForced(true);
        builder.setPositiveButton("Enable", new DialogInterface.OnClickListener() {
            public void onClick(DialogInterface dialog, int which) {
                startActivity(
                        new Intent(android.provider.Settings.ACTION_LOCATION_SOURCE_SETTINGS));
                Handler handler = new Handler();
                handler.postDelayed(new Runnable() {
                    public void run() {
                       enableGps();
                    }
                }, 5000);

            }
        });
        builder.setNegativeButton("Ignore", new DialogInterface.OnClickListener() {
            public void onClick(DialogInterface dialog, int which) {
                boolean enabled = lm.isProviderEnabled(LocationManager.GPS_PROVIDER);
                if(!enabled) {
                    showDialogGPS();
                }
            }
        });

        AlertDialog alert = builder.create();
        alert.show();

    }

    public void requestLocationPermission(){
        if(ActivityCompat.shouldShowRequestPermissionRationale(this,Manifest.permission.ACCESS_FINE_LOCATION)){
            ActivityCompat.requestPermissions(MainActivity.this,new String[]{Manifest.permission.ACCESS_FINE_LOCATION},LOCATION_REQUREST_CODE);
            }
            else
                ActivityCompat.requestPermissions(this,new String[]{Manifest.permission.ACCESS_FINE_LOCATION},LOCATION_REQUREST_CODE);
    }


    @Override
    public void onRequestPermissionsResult(int requestCode,String[] permissions,int[] grantResults) {

        if (requestCode == LOCATION_REQUREST_CODE) {
            if (grantResults.length > 0 && grantResults[0] == PackageManager.PERMISSION_GRANTED) {
                Toast.makeText(this, "permission granted", Toast.LENGTH_LONG).show();
                boolean enabled = lm.isProviderEnabled(LocationManager.GPS_PROVIDER);
                if(!enabled) {
                    showDialogGPS();
                }
            } else{
                Toast.makeText(this, "location access is necessary", Toast.LENGTH_LONG).show();
                Handler handler = new Handler();
                handler.postDelayed(new Runnable() {
                    public void run() {
                        requestLocationPermission();
                    }
                }, 3000);

            }
        }
    }


    public void enableGps(){
        boolean enabled = lm.isProviderEnabled(LocationManager.GPS_PROVIDER);
        if(!enabled) {
            showDialogGPS();
        }
    }

}
 
4.	Software Code
 package com.example.java.ewms;

import android.content.Intent;
import android.support.annotation.NonNull;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;

import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.auth.AuthResult;
import com.google.firebase.auth.FirebaseAuth;
import com.google.firebase.auth.FirebaseUser;
import com.google.firebase.database.DatabaseReference;
import com.google.firebase.database.FirebaseDatabase;

public class RegistrationActivity extends AppCompatActivity {
    private EditText userName, userPassword, userEmail;
    private Button regButton;
    private TextView userLogin;
    private FirebaseAuth firebaseAuth;
    private EditText userPhone;
    private DatabaseReference saveData = FirebaseDatabase.getInstance().getReference().child("users");


    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_registration);

        userName= (EditText)findViewById(R.id.etUserName);
        userPassword= (EditText)findViewById(R.id.etUserPassword);
        userEmail= (EditText)findViewById(R.id.etUserEmail);
        regButton= (Button)findViewById(R.id.btnRegister);
        userLogin= (TextView)findViewById(R.id.tvUserLogin);
        userPhone = (EditText) findViewById(R.id.etUserPhone);

                firebaseAuth=FirebaseAuth.getInstance() ;
        regButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                if (validate()) {
                    // Upload the Data to the DataBase
                    String user_email=userEmail.getText().toString().trim();
                    String user_password =userPassword.getText().toString().trim();
                    firebaseAuth.createUserWithEmailAndPassword(user_email,user_password).addOnCompleteListener(new OnCompleteListener<AuthResult>() {
                        @Override
                        public void onComplete(@NonNull Task<AuthResult> task) {
                            if(task.isSuccessful()){
                                Toast.makeText(RegistrationActivity.this,"Registration Successfull",Toast.LENGTH_SHORT).show();
                                //save data to database
                                saveData();

                                startActivity(new Intent(RegistrationActivity.this,MainActivity.class));
                                }else {
                                Toast.makeText(RegistrationActivity.this,"Registration failed",Toast.LENGTH_SHORT).show();
                            }

                        }
                    });
                }
            }
        });
        userLogin.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                startActivity(new Intent(RegistrationActivity.this,MainActivity.class));
            }
        });
    }

    private Boolean validate(){
        Boolean result=false;
        String name=userName.getText().toString();
        String password=userPassword.getText().toString();
        String email=userEmail.getText().toString();
        String phone=userPhone.getText().toString();

        if(name.isEmpty() ||password.isEmpty() || email.isEmpty()){
            Toast.makeText(this,"please enter all the Details",Toast.LENGTH_SHORT).show();

        }else{
            result=true;

        }
        return result;
    }
    private void saveData(){
        String name=userName.getText().toString();
        String password=userPassword.getText().toString();
        String email=userEmail.getText().toString();
        String phone=userPhone.getText().toString();
        String newEmail=email.replace(".",",");
        DatabaseReference saveUserData = saveData.child(newEmail);
        saveUserData.child("Name").setValue(name);
        saveUserData.child("Email").setValue(email);
        saveUserData.child("Password").setValue(password);
        saveUserData.child("Phone No").setValue(phone);




    }
}

5.	Software Code
 package com.example.java.ewms;

import android.Manifest;
import android.content.Context;
import android.content.Intent;
import android.content.pm.PackageManager;
import android.graphics.Color;
import android.location.Location;
import android.location.LocationListener;
import android.location.LocationManager;
import android.net.ConnectivityManager;
import android.net.NetworkInfo;
import android.os.AsyncTask;
import android.os.Handler;
import android.support.v4.app.ActivityCompat;
import android.support.v4.app.FragmentActivity;
import android.os.Bundle;
import android.support.v4.app.FragmentTransaction;
import android.support.v7.app.ActionBar;
import android.support.v7.app.AppCompatActivity;
import android.util.Log;
import android.view.Menu;
import android.view.MenuItem;
import android.widget.Button;
import android.widget.TextView;
import android.widget.Toast;

import com.google.android.gms.location.FusedLocationProviderClient;
import com.google.android.gms.location.LocationServices;
import com.google.android.gms.maps.CameraUpdateFactory;
import com.google.android.gms.maps.GoogleMap;
import com.google.android.gms.maps.OnMapReadyCallback;
import com.google.android.gms.maps.SupportMapFragment;
import com.google.android.gms.maps.model.BitmapDescriptor;
import com.google.android.gms.maps.model.BitmapDescriptorFactory;
import com.google.android.gms.maps.model.LatLng;
import com.google.android.gms.maps.model.Marker;
import com.google.android.gms.maps.model.MarkerOptions;
import com.google.android.gms.tasks.OnSuccessListener;
import com.google.firebase.auth.FirebaseAuth;

import org.json.JSONObject;

import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.net.HttpURLConnection;
import java.net.URL;

import static android.Manifest.permission.ACCESS_FINE_LOCATION;

public class Maps1Activity extends AppCompatActivity implements OnMapReadyCallback {


    private GoogleMap mMap;
    private FirebaseAuth firebaseAuth;
    private FusedLocationProviderClient client;
    private double lattitude;
    private double longitude;
    Marker mymarker;

  //  fetch data from json
    private static final String TAG = "UsingThingspeakAPI";
    private static final String THINGSPEAK_CHANNEL_ID = "765164";
    private static final String THINGSPEAK_API_KEY = "443DBA1XK3HULNWM"; //GARBAGE KEY
    private static final String THINGSPEAK_API_KEY_STRING = "443DBA1XK3HULNWM";
    /* Be sure to use the correct fields for your own app*/
    private static final String THINGSPEAK_FIELD1 = "field1";
    private static final String THINGSPEAK_FIELD2 = "field2";
    private static final String THINGSPEAK_UPDATE_URL = "https://api.thingspeak.com/update?";
    private static final String THINGSPEAK_CHANNEL_URL = "https://api.thingspeak.com/channels/";
    private static final String THINGSPEAK_FEEDS_LAST = "/feeds/last?";
    TextView timeText,valueText;
    Button b1;
    String data="",singlepars ="",singlepars1="";
    String timeData,valueData;
    //.................//

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_maps1);
        firebaseAuth = FirebaseAuth.getInstance();

        //if no internet connection
        NetworkInfo info = (NetworkInfo) ((ConnectivityManager)
                this.getSystemService(Context.CONNECTIVITY_SERVICE)).getActiveNetworkInfo();
        if(info == null)
        {
            Toast.makeText(this,"no internet connection",Toast.LENGTH_LONG).show();
            finish();
            // System.exit(0);
        }

        // Obtain the SupportMapFragment and get notified when the map is ready to be used.
        SupportMapFragment mapFragment = (SupportMapFragment) getSupportFragmentManager()
                .findFragmentById(R.id.map);
        mapFragment.getMapAsync(this);

         while(mapFragment == null){
             mapFragment.getMapAsync(this);

         }


//json
        new FetchThingspeakTask().execute();



        LocationManager lm = (LocationManager) getSystemService(LOCATION_SERVICE);
        if (ActivityCompat.checkSelfPermission(this, Manifest.permission.ACCESS_FINE_LOCATION) != PackageManager.PERMISSION_GRANTED && ActivityCompat.checkSelfPermission(this, Manifest.permission.ACCESS_COARSE_LOCATION) != PackageManager.PERMISSION_GRANTED) {
            return;
        }
        Location location = lm.getLastKnownLocation(LocationManager.GPS_PROVIDER);
        Log.d("checkerror",lattitude+" ");
        final LocationListener locationListener=new LocationListener() {
            @Override
            public void onLocationChanged(Location location) {
                lattitude=location.getLatitude();
                longitude=location.getLongitude();
                Log.d("checkerror",lattitude+" ");
            }

            @Override
            public void onStatusChanged(String provider, int status, Bundle extras) {

            }

            @Override
            public void onProviderEnabled(String provider) {

            }

            @Override
            public void onProviderDisabled(String provider) {

            }
        };
        while (lattitude==0.0) {
            lm.requestLocationUpdates(LocationManager.GPS_PROVIDER, 0,0, locationListener);
            lattitude = location.getLatitude();
            longitude = location.getLongitude();
        }

    }

    private void Logout() {
        firebaseAuth.signOut();
        finish();
        startActivity(new Intent(Maps1Activity.this, MainActivity.class));
    }

    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        getMenuInflater().inflate(R.menu.menu,menu);
        return true;
    }

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        switch(item.getItemId()){
            case R.id.logoutMenu:{
                Logout();
            }
        }
        return super.onOptionsItemSelected(item);
    }



    /**
     * Manipulates the map once available.
     * This callback is triggered when the map is ready to be used.
     * This is where we can add markers or lines, add listeners or move the camera. In this case,
     * we just add a marker near Sydney, Australia.
     * If Google Play services is not installed on the device, the user will be prompted to install
     * it inside the SupportMapFragment. This method will only be triggered once the user has
     * installed Google Play services and returned to the app.
     */
    @Override
    public void onMapReady(GoogleMap googleMap) {
        mMap = googleMap;
        // Add a marker in Sydney and move the camera
        LatLng mylocation = new LatLng(lattitude, longitude);
        Log.v("gunjan", Double.toString(lattitude));

        mMap.addMarker(new MarkerOptions().position(mylocation).title("My location"));
        mMap.moveCamera(CameraUpdateFactory.newLatLngZoom(mylocation,15));


//     if(valueData!= null)
//     mymarker =    mMap.addMarker(new MarkerOptions().position(new LatLng(30.218610,75.696959)).title("Dumping yard").icon(BitmapDescriptorFactory.fromResource(R.drawable.images2)));

        mMap.setOnMarkerClickListener(new GoogleMap.OnMarkerClickListener() {
          @Override
          public boolean onMarkerClick(Marker marker) {
              if(mymarker.equals(marker))
                  startActivity(new Intent(Maps1Activity.this, Main2Activity.class));
              return false;
          }
      });


    }

    class FetchThingspeakTask extends AsyncTask<Void, Void, String> {
        //        protected void onPreExecute() {
//            t2.setText("Fetching Data from Server.Please Wait...");
//        }
        protected String doInBackground(Void... urls) {
            try {
                URL url = new URL(THINGSPEAK_CHANNEL_URL + THINGSPEAK_CHANNEL_ID +
                        THINGSPEAK_FEEDS_LAST + THINGSPEAK_API_KEY_STRING + "=" +
                        THINGSPEAK_API_KEY + "");
                HttpURLConnection urlConnection = (HttpURLConnection) url.openConnection();
                try {
                    BufferedReader bufferedReader = new BufferedReader(new InputStreamReader(urlConnection.getInputStream()));
                    StringBuilder stringBuilder = new StringBuilder();
                    String line;
                    while ((line = bufferedReader.readLine()) != null) {
                        data = data+line;


                    }
                    bufferedReader.close();
                    //data = stringBuilder.toString();
                    // singlepars = data.substring(38);
                    JSONObject json = new JSONObject(data);
                    timeData = json.getString("created_at");
                    valueData = json.getString("field1");
//                    singlepars ="Date: "+ json.getString("created_at")+"\n"+"value: "+json.getString("field1");
                    Log.v("mahesh",singlepars+"kffkd");
                    // singlepars = data.substring(data.)
                    return stringBuilder.toString();


                }
                finally{
                    urlConnection.disconnect();
                }
            }
            catch(Exception e) {
                Log.e("ERROR", e.getMessage(), e);
                return null;
            }
        }
        protected void onPostExecute(String response) {
//            if(response == null) {
//                Toast.makeText(Main2Activity.this, "There was an error", Toast.LENGTH_SHORT).show();
//                return;
//            }
//            try {
//                JSONObject channel = (JSONObject) new JSONTokener(response).nextValue();
//                double v1 = channel.getDouble(THINGSPEAK_FIELD1);
//                if(v1>=90)
//                    t1.setText("HI ALL  ");
//                else
//                    t1.setText("NO VALUES");
//            } catch (JSONException e) {
//                e.printStackTrace();
//            }
//            if(data == null)
//            { Toast.makeText(Maps1Activity.this,"no data available",Toast.LENGTH_SHORT).show();
//                return;}
//
//            timeText.setText(timeData);
//            if(Integer.parseInt(valueData)<=30)
//                valueText.setTextColor(Color.parseColor("#2e7d32"));
//            else
//            if(Integer.parseInt(valueData)>30 && Integer.parseInt(valueData)<=60)
//                valueText.setTextColor(Color.parseColor("#ffab00"));
//            else
//                valueText.setTextColor(Color.parseColor("#d50000"));
//            valueText.setText(valueData);

            if(Integer.parseInt(valueData)<=30)
                mymarker =  mMap.addMarker(new MarkerOptions().position(new LatLng(30.218610,75.696959)).title("Dumping yard").icon(BitmapDescriptorFactory.fromResource(R.drawable.sssss)));
            else
                if(Integer.parseInt(valueData)>30 && Integer.parseInt(valueData)<=60)
                    mymarker =    mMap.addMarker(new MarkerOptions().position(new LatLng(30.218610,75.696959)).title("Dumping yard").icon(BitmapDescriptorFactory.fromResource(R.drawable.yellow1)));
                else
                    mymarker =    mMap.addMarker(new MarkerOptions().position(new LatLng(30.218610,75.696959)).title("Dumping yard").icon(BitmapDescriptorFactory.fromResource(R.drawable.red)));

        }
    }

}




























CONCLUSION

In this project, an integrated system of GSM/GPRS module, Arduino and Ultrasonic Sensor is introduced for efficient and economic garbage collection. The developed system provides improved database for garbage collection time and waste amount at each location. By implementing this project we will avoid over flowing of garbage from the container in residential area which is previously either loaded manually or with the help of loaders in traditional trucks. It can automatically monitor the garbage level & send the information to collection truck. The technologies which are used in the proposed system are good enough to ensure the practical and perfect for solid garbage collection process monitoring and management for green environment.

We have successfully completed the project “DEVELOPMENT OF SMART DUMPYARD AND WASTE MONITORING SYSTEM”, but, there’s still room for change.

•	For instance, we intend to expand our model and make it more dynamic.
•	Our model works on the assumption that there’s only one collecting truck. This can be implemented on a larger scale, with more collector trucks, given the required funds and time.
•	We also intend to make our routing algorithm better and more efficient.
 

Future Enhancement


Automatic Garbage Fill Alerting system helps us to reduce the pollution. Many times garbage dustbin is overflow and many animals like dog or cow enters inside or near the dustbin. Also some birds are also trying to take out garbage from dustbin. This project can avoid such situations. And the message can be sent directly to the cleaning vehicle instead of the contractor’s office. Apart from this, differentiation can be made between dry trash bin and wet trash bin collecting plastic dry waste and biodegradable waste respectively. To implement this methane and smell sensors can be used. This helps in distinguishing the waste at the source and hence reducing the requirement of manpower. To enhance it further, an automated system can be developed which is able to pick up waste in and around the bin, segregate them and put them in respective bins.























REFERENCES 

•	Navghane S S, Killedar M S and Rohokale D V 2016 IoT Based Smart Garbage and waste collection, International Journal of Advanced Research in Electronics And Communication.
•	Monika K A, Rao N, Prapulla S B and Shobha G 2016 Smart Dustbin-An EfficientGarbage Monitoring System International Journal of Engineering Science andComputing 6 7113-16.
•	 Medvedev A, Fedchenkov P, Zaslavsky A, Anagnostopoulos T and Khoruzhnikov S,2015 Waste management as an IoT-enabled service in smart cities In Conference on Smart Spaces Springer International Publishing 104-15.
•	www.buildofy.in/smart_home_designs 
•	https://create.arduino.cc/projecthub/Technovation/smart-garbage-monitoring-systemusing-arduino-101-3b813c  
•	https://github.com/sourabhdeshmukh/Smart-Dustbin
•	https://www.google.com/imgres?imgurl=https%3A%2F%2F5.imimg.com%2Fdata5%2FXT%2FON%2FMY-10360035%2Fwaterproof-ultrasonic-sensor-jsn-sr04t-distance-transducer-sensor-for-arduino-500x500.jpg&imgrefurl=https%3A%2F%2Fwww.indiamart.com%2Fproddetail%2Fwaterproof-ultrasonic-sensor-jsn-sr04t-distance-transducer-sensor-for-arduino-20421146148.html&tbnid=tAy1P0pnxdaPgM&vet=1&docid=KseyplgMjJZN-M&w=500&h=499&q=jsn%2004%20ultrasonic%20sensor.&hl=en-IN&source=sh%2Fx%2Fim
•	https://images.app.goo.gl/hycpdauGnGR5vMjQ6
•	https://firebase.google.com/docs/app-indexing/


