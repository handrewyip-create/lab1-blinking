#include "mbed.h"

// Blinking rate in milliseconds
#define BLINKING_RATE     200ms
    // Initialise the digital pins LED1, LED2 and LED3 as output
    DigitalOut led(LED1);
    DigitalOut led2(LED2);
    DigitalOut led3(LED3);

void sequence() //declare the function
{   //the 'ping-pong' sequence
    led = 1; 
    ThisThread::sleep_for(BLINKING_RATE);
    led = 0; 
    ThisThread::sleep_for(BLINKING_RATE);
    
    led2 = 1; 
    ThisThread::sleep_for(BLINKING_RATE);
    led2 = 0; 
    ThisThread::sleep_for(BLINKING_RATE);

    led3 = 1; 
    ThisThread::sleep_for(BLINKING_RATE);
    led3 = 0; 
    ThisThread::sleep_for(BLINKING_RATE);

    led2 = 1; 
    ThisThread::sleep_for(BLINKING_RATE);
    led2 = 0; 
    ThisThread::sleep_for(BLINKING_RATE); //led1 will blink next in the loop
}

int main()
{
    while (true) {
    sequence(); //call the function inside the loop
    }
}
