#include "mbed.h"

// Blinking rate in milliseconds
#define BLINKING_RATE     200ms
    // Initialise the digital pins LED1, LED2 and LED3 as output
    DigitalOut led(LED1);
    DigitalOut led2(LED2);
    DigitalOut led3(LED3);

void OnOff() //declare the function
{   //turns the leds on together 
    led = 1; 
    led2 = 1;
    led3 = 1; 
    ThisThread::sleep_for(BLINKING_RATE);//on for 200ms
    //turns the leds off together
    led = 0; 
    led2 = 0;
    led3 = 0;
    ThisThread::sleep_for(BLINKING_RATE);//off for 200ms
}

int main()
{   
    int repeat5 = 0;
    
    while (true) {
    OnOff(); //call the function inside the loop
    repeat5++;//keep +1 
    
    if (repeat5 >= 5) break; //ends the loop if 'repeat5' is bigger than 5
    }
    // turns led1 on and led2 and led3 remain off
    led = 1;
    led2 = 0;
    led3 = 0; 
}
