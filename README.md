# Stereo out test using Cirrus CS4271 and STM32G474CEU6

Pinouts  
![](/pins.png)

PC6 is used for blinking the onboard LED if an error has occured.  
I2C pins needs 4.7k pullup resistors.

See CS4271 datasheet for connection diagram.  
[CS4271](https://www.cirrus.com/products/cs4271)

# SAI
- 16 bits signed integer
- datasize 16
- frl 32
- slots 2
- activelength 1

# Memory
Buffer needs to be locate in SRAM2 to avois cache something something. 

# DMA
Sai dma, half-word circular
