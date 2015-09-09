# emPC-A/RPI by Janz Tec AG
**Low Cost ARM Cortex-A7 Based Embedded Controller**

On our [website](https://www.janztec.com/en/empc-a-rpi.html), the binary emPC-A/RPI driver package is available in the download area. This Raspbian compatible .deb package includes all compiled drivers, kernel modifications and configuration entries to enable the additional features of the emPC-A/RPI (RTC, CAN, RS232/RS485), and is based on the source code modifications included in this repository. 

Product page: https://www.janztec.com/en/empc-a-rpi.html
![emPC-A/RPI](https://www.janztec.com/uploads/tx_templavoila/emPC-A_RPI_neu_642x480.jpg)

**FEATURES emPC-A/RPI**
* Processor 
  * Based on Raspberry Pi 2, Model B 
  * Broadcom BCM2836 processor 
  * Quad-Core CPU based on ARM Cortex-A7  with 900 MHz 
  * Fanless cooling concept 
  * Realtime clock, battery buffered 
* Memory 
  * System memory 1 GB 
  * External accessible µSD card slot  
* Graphics 
  * HDMI graphic interface  
* Connectors  
  * 1 x 10/100 MBit/s Ethernet 
  * 4 x USB (v2.0) 
  * 1 x 9-pin D-SUB connector for serial debug console 
  * 1 x CAN (ISO/DIS 11989-2, opto-isolated, termination settings via jumper) 
  * 1 x RS232 (Rx, Tx, RTS, CTS) or switchable to RS485 (half duplex; termination settings via jumper)  
  * Internal I/O  
    * 4 x digital inputs (24VDC) 
    * 4 x digital outputs (24VDC)  
* Power Supply  
  * Input 9 … 32 VDC 

for more information on how to compile this repository visit https://github.com/raspberrypi/linux/blob/rpi-3.18.y/README

Before compiling this kernel sources, make sure that the following entries are configured as *modules* in "menuconfig":
* (M) Microchip MCP251x SPI CAN controllers 
* (M) BCM2798 SPI controller driver (SPI0)
* (M) User mode SPI driver support 
* (M) SC16IS7xx serial support 
* (M) Dallas/Maxim DS1307/37/38/39/40, ST M41T00, EPSON RX-8025 
