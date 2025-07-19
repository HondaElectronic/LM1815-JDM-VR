# LM1815-JDM-VR 0.1v
There are some considerations and updates to this design, its just 0.1version

Didn't test it on the car yet but should work, with signal generator it looks like it's working

I finished it some time ago but didn't upload on github

This is designed for speeduino platform

The design is bulky and THT since its a first prototype

## Use case ##
* 24+1 dual wheel setups
* 12+1
* Probably like Mazda RX7 systems will also work, not sure

## Limitations ## 
* Lm1815 is old, slow and expensive IC but it's easy to implement and it work's with 24+1 honda distributor most of the time
* The rise time is very fast, around 5ns, it generates some spikes in output signal, not sure if its problem with my equipment, cables or this is design restriction 

## Specs ##
* It will work with signal as low as 100mV p-p
* Reasonably fast and accurate
* Fairly cheap compared to commercial products
* Should work up to 12,5k rpm's but tested it way higher and looked like it worked
* The schmitt trigger is not needed but it helps with noise reluctance and generating faster rise times and fall times

## Considerations ##
* Doing proper SMD board
* The schmitt trigger is super tiny, you need some experiance with smd hotair soldering to not overheat it, you should  solder it first or redesign the board for bigger one
* You could use non inverting schmitt trigger and probably should

THIS DESIGN IS ONLY FOR NON PROFIT PRIVATE MOTORSPORT USE ONLY

## LM1815 output vs schmitt trigger output ##

![PXL_20250719_115934090 MP](https://github.com/user-attachments/assets/7f0dafd9-1ce3-4eb8-b5ed-4efe199aa192)

## Ringing of the output signal ##
![PXL_20250709_221349925](https://github.com/user-attachments/assets/d3d6013a-c50f-4639-8db5-c559b960c8c5)

## Schmitt trigger vs the rest of the board ##
![PXL_20250702_194544577](https://github.com/user-attachments/assets/1f5714ef-a352-4355-bf52-b43edb8a552d)

## Assembled board ##
![PXL_20250705_225356400](https://github.com/user-attachments/assets/78d6054a-0dec-4ca4-8428-2c6d844de678)

