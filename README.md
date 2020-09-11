
|  Hack Club Malagon Staff|  
|--|--|
| @Andrei | 
|@Miruna
|@Olga




# Keep your distance

> A simple project to introduce your **Hack Club** to the world of `Arduino` and `Robotics`
 
If you want people to maintain a **secure distance** this is your project 🥰!

  
  

## About this amazing project 💖

  

This is a simple workshop which hooks a HC-SR04 Ultrasonic Sensor to the Arduino Uno & alarms you when someone is close by turning on the LEDs.

  

## How it works 🙋?

  

The idea behind it’s very simple: the sensor emits an ultrasound at 40 000 Hz which travels through the air and if there is an object or obstacle on its path it will bounce back to the module. Considering the travel time and the speed of the sound you can calculate the distance. If the object is in our range then triggers a visual(LEDs) alarm.


**![](https://lh6.googleusercontent.com/XsrrayIPFLd1bVmLmnS5KHaBSCZFRA2Q6n1-LT72H1tRephAIQ-EFYG6CR9Q_P7CiiybLQX4-tQyHVH-K7h1cb1hyOe_a33VbYYgGWJZLxGixErPWP1dOpvX4Y4RKkU9uKo8xhI)**
**![Imagen relacionada](https://lh3.googleusercontent.com/qwWq9KDQn-BS05KCQpTsYLFMfR1_GEIUCvwxKJf9Nv4m4bdvUY2oBEHMUgkmfVBo3m5Ep-7mXzOyKJ2GJc3W3-LzP6aBPo-50j1cKmB_RZlPBtRD_XMswhurmFQj1z75HALYECI)**


## Equipment needed 🧙‍♀️:

In this project you won’t be needing nothing fancy😎. They are all in the Arduino kit and should be easy to find online or in your nearby electronics/hobby shop or even your high school 🏫 has them!

-   **Arduino UNO.**
    **![](https://lh3.googleusercontent.com/WZXEqy0C0XOkFpfeGdDAn6_qwguOV-mhSeKc2VHn8agF0oBL8C35QO7Km9DiGnhSmOSQm5dN5Gs6ac5ZuBjfdPaVnFIZUE6N57Y45YrAHh3rP8ZnqpHO9fon79zpp25IXEA-rYP5)**
-   **Protoboard.**
    **![](https://lh3.googleusercontent.com/0FOTTy8hM-SdssOCsOoPVZSNMOyjTA6rPLNo8TS9jm4X7TbGOvzukcwRu51ivKJt7BrftxsnhoGqL2mI9iKIVku6u4nR6QJjCH4QnK7JmLJpBCxawKFEG_vkzRHM0GXpTDdQbRvy)**
-   **14 jumper wires.**
    **![](https://lh4.googleusercontent.com/RKOw0355w887KaXiTqlpKhky9sAQMtgXcP2dpQMHlpSdCML_Wv98jkWNMPSdc7wsIHXZ5Pq5nUq780nafOyCtS3B0al91WhzDCGkBYEP47Ntzn6wtDCkKv7q5CEJ0HCb92882htV)**
-   **3ª 220 Ω resistors.**
    **![](https://lh5.googleusercontent.com/DJFalZKPsuYLEIDbaO9UZBBlPWElH2uz21Oetca3pUZDiEnGE1cGeb42aG1ras35JyceXUhSyGz-tGgyVNsZ0i6i8hnnroleDs-9A91-jhl4KaLWU0rmUd4-LDcfF187kbhD-V1z)**
-   **1 green LED, 1 yellow LED, 1 red LED.**
    **![](https://lh5.googleusercontent.com/CP2L8eiMzViMNm3fnuUjT0c7k-WwrkcliIVnaerPnDBWlNmdf8HdCdlaPPx-9M1WbpjaowId4vsFmBQbkONcctv5GqmRnHCKsHwGqF-w_-kQvNQIPhRdSKp1uvxs-O1cDvZoL4pp)**
-   **1 Arduino Ultrasonic Sensor (HC-SR04).**
    **![](https://lh4.googleusercontent.com/UnGPhpeOPziKuAszXYJ8wM8zGr3HWmaEUihQVaCAK_rrni2uAcSubA8bQj2iPn7MJM5Xj_WdChK-q5odPDTDz_YdWTwPAaSn-m2rn6HskeLGMPGfR51P2rb4yLyl6xLTucvC1Hxn)**
    


## Steps you have to follow 🤖

  
  

**Let’s start by connecting the LEDs:**

  

1.  First put all the **LEDs** on the **ProtoBoard** as you can see in the image.
    
2.  Connect the **positive** side of the LEDs (the long one) to the pins with a black/blue line on the Protoboard. Remember to connect the resistors between the **negative** side of the LED and the cable that goes to the Protoboard.
    
3.  Connect a cable that goes from the pins with a black line of the breadboard to the GND pin of the **Arduino UNO**
    
4.  Connect each **negative** side of the LEDs to the pins 2, 3 and 4.
    
5.  Connect the series of pins with a red line from the Protoboard to the **5v pin** of the Arduino UNO.
    

![](https://lh5.googleusercontent.com/O6f7zqATS4sB8n1MMdG4lKeSMgfsgzsXcMJqz0ATyXPrC6a5KzgCAEGray_kJHEwuQwDtR1VzVVBPR5MPp6O4gF3DRsY9S8OtghDufm52VjkesxdcmJUgrfpLIzwQdyxbgE_YhMo)

  
  
  
  
  
  

**Let's continue connecting the proximity sensor to the Arduino UNO:**

  
  
  

1.  First we need to connect the `VCC` pin from the sensor to the pins with a **red line** of the protoboard.
    
2.  Connect the `GND` pin of the sensor to the pins with a **black/blue line** of the protoboard.
    
3.  Connect the `Trig` pin from the sensor to the `5th` **digital pin** of the Arduino UNO. This pin will send the **ultrasonic pulse**.
    
4.  Connect the `Echo` pin from the sensor to the `6th` **digital pin** of the Arduino UNO. This pin will send **information** to the Arduino UNO.
    

  

![](https://lh5.googleusercontent.com/8fTOl1ccwiseKiMUB5OPrckb8H-DJjLwHBMmZXmsnj0fg7q9XTMhUAcvpN5XiRrjPZpYvluHIIegHzIBw4MhJv_GyN_cjqOqRGflmGRH9kWl2zUrU5Tjb6sGsazdexRUjItUVLaF)

  
  
  
  
  

## The code

  

Here's the code. I added comments throughout the codes so that is easier to follow! Take a look below or download it [here](https://github.com/hackclub/hackclub/blob/main/workshops/line_following_robot/blahbalh.com).


Start by defining the **pins** that we are using for the **LEDs** and the **proximity sensor**.
Next, we establish some parameters for the **LED alerts**. You can edit the parameters to your liking, as well as the pins defined in case you have used others.

    #define GREENLED 2
    #define YELLOWLED 3
    #define REDLED 4
    #define TRIGGER 5
    #define ECHO 6
    
    
    
    const float sound = 34300.0; // Sound speed in cm / s
    const float parameter1 = 30.0;
    const float parameter2 = 20.0;
    const float parameter3 = 10.0;


We turn on the `Serial Begin` at **9600** bits per second (this will allow us to communicate with the sensors through the arduino and see the data in the **Serial Motor**).
Below, we establish the **input / output** of each component, in the case of the **LEDs** and the **Trigger** we only need to **send** information (in this case electricity), that is why we establish the `OUTPUT`. Instead, we set the **ECHO** to `INPUT` since we want to **receive** information from that pin. 

    void setup() {
   
      Serial.begin(9600);
    
      // Pin input / output mode
      pinMode(GREENLED, OUTPUT);
      pinMode(YELLOWLED, OUTPUT);
      pinMode(REDLED, OUTPUT);
      pinMode(ECHO, INPUT);
      pinMode(TRIGGER, OUTPUT);
      
    
      // Turn off all the LEDs
      turnOffLEDs();
    
    }




In the following code we define the functions that we are going to use. First we define the **function to turn off all the LEDs** and then the function of the `alerts`. This is a very simple and easy code.



    // Turn Off All the LEDs
    void turnOffLEDs()
    {
      // First, we turn off all the LEDs
      digitalWrite(GREENLED, LOW);
      digitalWrite(YELLOWLED, LOW);
      digitalWrite(REDLED, LOW);
    }
    
    // Function that checks if a visual or sound alert needs to be launched
    void alerts(float distance)
    {
      if (distance < parameter1 && distance >= paremeter2)
      {
        // Turn on GREEN LED
        digitalWrite(GREENLED, HIGH);
        
      }
      else if (distance < parameter2 && distance > parameter3)
      {
        // Turn on YELLOW LED
        digitalWrite(YELLOWLED, HIGH);
        
      }
      else if (distance <= parameter3)
      {
        // Turn on RED LED
        digitalWrite(REDLED, HIGH);
       
      }
    }

  
In the next part of the `code` we define the function to calculate the distance that we want to measure with the **proximity sensor**.
Within the code itself there are comments explaining each part more thoroughly.
We then define the function that will allow the proximity sensor to measure the distance, first we ask it to be off, then we turn it on (for which it sends an **ultrasonic pulse**), and finally we turn it off.


    // Method that calculates the distance an object is located.
    // Returns a float variable that contains the distance.
    float calculateDistance()
    {
      // The pulseIn function gets the time it takes to switch between states, in this case HIGH
      unsigned long times = pulseIn(ECHO, HIGH);
    
      // We obtain the distance in cm, we have to convert the time in seconds since it is in microseconds
      // so multiply by 0.000001
      float distance = times * 0.000001 * sonido / 2.0;
      Serial.print(distance);
      Serial.print("cm");
      Serial.println();
      delay(500);
    
      return distance;
    }
    
    // Method that starts the Trigger sequence to start measuring
    void startTrigger()
    {
      // Put the Trigger in low state and wait 2 ms
      digitalWrite(TRIGGER, LOW);
      delayMicroseconds(2);
    
      // Put the Trigger pin high and wait 10 ms
      digitalWrite(TRIGGER, HIGH);
      delayMicroseconds(10);
    
      // Start by putting the Trigger pin in low state
      digitalWrite(TRIGGER, LOW);
    }




## Here is the complete code.


    // Defined Pins
    #define GREENLED 2
    #define YELLOWLED 3
    #define REDLED 4
    #define TRIGGER 5
    #define ECHO 6
    
    
    // parameters
    const float sound = 34300.0; // Sound speed in cm / s
    const float parameter1 = 30.0;
    const float parameter2 = 20.0;
    const float parameter3 = 10.0;
    
    void setup() {
      // Start the serial monitor
      Serial.begin(9600);
    
      // Pin input / output mode
      pinMode(GREENLED, OUTPUT);
      pinMode(YELLOWLED, OUTPUT);
      pinMode(REDLED, OUTPUT);
      pinMode(ECHO, INPUT);
      pinMode(TRIGGER, OUTPUT);
      
    
      // Turn off all the LEDs
      turnOffLEDs();
    
    }
    
    void loop() {
      // Prepare the ultrasound sensor
      startTrigger();
    
      // Obtain Distance
      float distance = calculateDistance();
    
      // Turn off all the LEDs
      turnOffLEDs();
    
      // We launch an alert if we are within the danger range
      if (distance < parameter1)
      {
        // Lunch alerts
        alerts(distance);
      }
    
    }
    
    // Turn Off All the LEDs
    void turnOffLEDs()
    {
      // First, we turn off all the LEDs
      digitalWrite(GREENLED, LOW);
      digitalWrite(YELLOWLED, LOW);
      digitalWrite(REDLED, LOW);
    }
    
    // Function that checks if a visual or sound alert needs to be launched
    void alerts(float distance)
    {
      if (distance < parameter1 && distance >= paremeter2)
      {
        // Turn on GREEN LED
        digitalWrite(GREENLED, HIGH);
        
      }
      else if (distance < parameter2 && distance > parameter3)
      {
        // Turn on YELLOW LED
        digitalWrite(YELLOWLED, HIGH);
        
      }
      else if (distance <= parameter3)
      {
        // Turn on RED LED
        digitalWrite(REDLED, HIGH);
       
      }
    }
    
    // Method that calculates the distance an object is located.
    // Returns a float variable that contains the distance.
    float calculateDistance()
    {
      // The pulseIn function gets the time it takes to switch between states, in this case HIGH
      unsigned long times = pulseIn(ECHO, HIGH);
    
      // We obtain the distance in cm, we have to convert the time in seconds since it is in microseconds
      // so multiply by 0.000001
      float distance = times * 0.000001 * sonido / 2.0;
      Serial.print(distance);
      Serial.print("cm");
      Serial.println();
      delay(500);
    
      return distance;
    }
    
    // Method that starts the Trigger sequence to start measuring
    void startTrigger()
    {
      // Put the Trigger in low state and wait 2 ms
      digitalWrite(TRIGGER, LOW);
      delayMicroseconds(2);
    
      // Put the Trigger pin high and wait 10 ms
      digitalWrite(TRIGGER, HIGH);
      delayMicroseconds(10);
    
      // Start by putting the Trigger pin in low state
      digitalWrite(TRIGGER, LOW);
    }
      

## Final Result 🥳!

  

![](https://lh6.googleusercontent.com/SE-vqqEXLu9AvZyGejMHjlSsiybfRQYE8S9HvJ5aznCxT8tDsPJ7pEZBNbWbtoF_JMaWcyg34jjUURyG2XL4ySoOgZ0hpEdUdf41ENh_mLjSlhLauZ0huYlYLNhPxyJBIFLF1Nnt)![](https://lh5.googleusercontent.com/Owh5KfrBe6cABvryhnXOtsEJ_LsDSRL_vgSKUVjKnIluSlSlW7baIcX6wH907-u6RYRLyIJPyuc4NsRLAz9KQTU1-kHHwMa6-Pm9nxmWrSAhBbWyjbw5OnTOFdKn-TzpJ3tLgwhQ)

  

You’ll have your `arduino proyect` running and keeping others away! 😂😂










