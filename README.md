# blinkmini-re

Reverse engineering an Amazon Blink Mini to repurpose in future projects.

A vast majority of this *mini* project (pun intended) is based on this [blog post](https://astrid.tech/projects/blink-mini-re/). Unfortunately, this series seems to have ended before getting the Blink Mini into a re-usable state but that is where I will attempt to continue.

## Disassembly
Similar execution to the previously linked blog post. 

## Dumping the ROM
I already had a CH341a SPI programmer from a previous mini project where I dumped the BIOS chip of a ThinkPad I had purchased off eBay that had unfortunately come with a BIOS admin password that the seller did not know. Instead of sending it back, I went with the more fun approach and dumped the BIOS, modified a version of the stock BIOS to get additional settings, then re-flashed with the motherboard's BIOS chip. 
Unlike the blogger, I decided to wait until I received the appropriate tools from Aliexpress before continuing. 

`sudo flashrom --programmer ch341a_spi -r flash.bin`

### Dependencies
`sudo apt install flashrom binwalk`

## Analyzing the binary

## Repurposing

