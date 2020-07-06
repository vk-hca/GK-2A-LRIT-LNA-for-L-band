# GK-2A-LRIT-LNA-for-L-band

Just some notes and an example of converting a cheap S band TV LNB into an L band LNA for use on on the Korean GK-2A weather satelite but also useful for any other 
L band linear polarisation use like the GOES and other L band satellites.

Switching between vertical and horizontal polarisations is aheived by changing the supply voltage on coax from 12v to 18v as in the normal satelite TV LNB usage.

These S band LNBs are used on the SES7 at 108.2E MNC / Indovision 2.5 ghz signal which is possibly the only direct brodcast satelite to use S band, availiblity is local to Indonesia from many online shops selling DVB-S2 set top recievers and associated equipment for around the $10 dollar mark.

It works fine with an RTL-SDR requiring only an inline power injector or bias tee, the 5v bias tee output of an sdr is not suitable.

Mounted offest in a 1.8mt C band dish with the prime C band LNB set on Telstar vantage at it works fine with 100 metres of RG11 cable run to the V3 RTL-SDR 
using the software provided by this LRIT project on github. https://vksdr.com/xrit-rx

