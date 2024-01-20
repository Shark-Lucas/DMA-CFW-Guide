# DMA-FW-Guide
The following guide previews detailed instructions on the creation of modified DMA (attack) Firmware based on [pcileech](https://github.com/ufrisk/pcileech). <br />

#### 📖Why make this guide?
I know how tedious reading through pages of threads and documentation can be to make some relatively minor changes such as this,
additionally, it doesn't help that there are people intentionally being vague and keeping information secret, or even misleading 
people to push them to buy their +$100 "highly custom undetectable" firmware.

### ⚠️ Disclaimer
(Don't expect this to work for Vanguard, Faceit, ESEA, or other such sophisticated ACs as they are much more 'intrusive'. <br />
Also, this guide does ___not___ detail how to set up software or change computer settings to accommodate DMA cards)




### 📑 CONTENTS
1. [Requirements](https://github.com/Silverr12/DMA-FW-Guide#1-requirements)
2. [Gathering the donor information](https://github.com/Silverr12/DMA-FW-Guide#2-gathering-the-donor-information)

## **1. Requirements**


#### Download
- [Visual Studio](https://visualstudio.microsoft.com/vs/community/)
- [Xilinx Vivado](https://www.xilinx.com/support/download.html)
- [Pcileech-fpga](https://github.com/ufrisk/pcileech-fpga) source code for custom firmware
- [RWEverything](http://rweverything.com/download/)





## **2. Gathering the donor information** 
Due to my limited testing and knowledge, I'll be using a network adapter for all examples continuing <br />
<sup>(I welcome any contribution about utilising different hardware for this)</sup>

### Using RWEverything
- Press PCI Devices in the top left and navigate the list to find your donor card
- Once in here, under "Summary" on the right-hand side, take note of the:
1. Device & Vendor ID, under Summary it will display for example as _0x2G4H5302_, disregarding the 0x, the first 4 letters/numbers are your Device ID, and the other 4 the Vendor ID.
2. Revision ID
3. BAR1
4. Subsystem ID, but only the first 4 letters/numbers once again as the other 4 are duplicates of our Vendor ID
5. Either take a picture of the block of bytes underneath the dropdown or save the dump as a file













### Additional Credits
garagedweller's [UC thread](https://www.unknowncheats.me/forum/anti-cheat-bypass/613135-dma-custom-firmware-guide.html) <br />
Ulf Frisk for [pcileech](https://github.com/ufrisk/pcileech) <br />
ekknod for his [custom pcileech config](https://github.com/ekknod/pcileech-wifi) <sub>(I recommend looking into this further if you want to look towards creating firmware to bypass sophisticated ACs)</sub>

