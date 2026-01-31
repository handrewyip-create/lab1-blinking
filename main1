#include "mbed.h"

// Blinking rate in milliseconds
#define BLINKING_RATE     500ms

int main()
{
    // Initialise the digital pins LED1, LED2 and LED3 as output
#ifdef LED1, LED2, LED3
    DigitalOut led(LED1);
    DigitalOut led2(LED2);
    DigitalOut led3(LED3);
#else
    bool led, led2, led3;
#endif

    while (true) {
        led = !led;
        led2 = !led2;
        led3 = !led3;
        ThisThread::sleep_for(BLINKING_RATE);
    }

}
