# Verification Testing

 This code will create a task to run a verification test on the system.
 The system samples a voltage using an ADC every five seconds,then from the ADC output, calculates and prints the voltage to the terminal
 Unit Under Test: adcResToVoltage() which determines whole and fractional part of voltage value corresponding to an ADC result

# Important Files

 Source file: main/user_main.c,
 Output file: main/lab3_q3_816005001.out,
 Binary file: build/i2c.bin

# Test file

 There is no explicit test file. The verification_test_task in main/user_main.c does the job of a test driver in this code.
 There is only one test case: where the voltage at the ADC input is 2.85V.
 There is only one test case because when the serial monitor output is being saved to a file, one cannot see the
 messages being output by the program and hence one cannot know what test case the program expects next.

# Pin Assignment

* Master (ESP8266):
    * GPIO2 is assigned as the data signal of i2c master port
    * GPIO0 is assigned as the clock signal of i2c master port

# Hardware Required

 Connection: connect sda/scl of sensor with GPIO2/GPIO0

# Example Output  
  
```

I () main: Verification testing task

I () main: UUT: whole system: system samples a voltage using an ADC every five seconds,
                calculates and then prints the voltage to the terminal

I () main: Please set voltage to 2.85V. I will wait for 5s...

I () main: Now sampling...

I () main: ADC Result: 0x9250 [37456]

I () main: Expected voltage -> Whole: 2, Fraction: 13600 / 16000 V

I () main: Voltage -> Whole: 2, Fraction: 5456 / 16000 V

```
