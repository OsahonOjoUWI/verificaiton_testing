# I2C Example

 This example shows how to use I2C for inter-device communication.

# Important Files

 Source file: main/user_main.c
 Output file: main/lab1_q3_816005001.out
 Binary file: build/i2c.bin

# Pin Assignment

* Master (ESP8266):
    * GPIO2 is assigned as the data signal of i2c master port
    * GPIO0 is assigned as the clock signal of i2c master port

# Hardware Required

 Connection: connect sda/scl of sensor with GPIO2/GPIO0

# Example Output  

```

I (0) gpio: GPIO[2]| InputEn: 0| OutputEn: 1| OpenDrain: 1| Pullup: 0| Pulldown: 0| Intr:0
I (0) gpio: GPIO[0]| InputEn: 0| OutputEn: 1| OpenDrain: 1| Pullup: 0| Pulldown: 0| Intr:0
Inside app_main
Inside task_example

I (0) main: ADC Result: xxxx

I (0) main: ADC Result: xxxx

I (0) main: ADC Result: xxxx

```
