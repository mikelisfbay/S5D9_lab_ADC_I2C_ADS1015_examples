# S5D9_lab_ADC_I2C_ADS1015_examples
This is a set of examples that show how to add the ADC capability to the S5D9 IOT board.

This board has two grove headers.  Grove B is an IIC port while grove A is an SCI port.   You creates r_iic driver for the IIC port and r_sci_i2c for the SCI port.  

6 examples are included in this tutorial.

1. Grove B / r_iic driver (only for the fast speed mode) *
2. Grove B / framework with r_iic driver
1. Grove A / r_sci_i2c driver
2. Grove A / framework with r_sci_i2c driver

* Because r_iic has some issue for standard speed mode. Two possible workaround examples are included.
1. Grove B / r_iic driver / method 1 with busy bit check
2. Grove B / r_iic driver / method 2 with busy bit check

Both checks for the hardware busy bit before the code starts the next i2c transmission.   The above examples are are done with limited testing.  At this point, this ADC component seem to work well with these workaround solutions. 

Files in this repository:

S5D9_lab_ADC_I2C_ADS1015_examples.zip (Renesas Snergy projects' zip file)

S5D9 ADS1015 I2C ADC Tutorial Summary.pdf (Tutorial Summary)

ads1015.pdf (TI ADS 1015 Datasheet)

ADC module

ADS1015 12-Bit ADC - 4 Channel with Programmable Gain Amplifier

https://www.adafruit.com/product/1083

Lastly, here is my blog.

https://www.miketechuniverse.com/single-post/2018/03/02/Add-ADC-to-S5D9-IOT-board
