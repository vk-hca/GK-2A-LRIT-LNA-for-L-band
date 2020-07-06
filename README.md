# GK-2A-LRIT-LNA-for-L-band

Just some notes and an example of convering an S band LNB into an Lband LNA for use on on the Korean GK-2A weather satelite but also useful for any other 
L band linear polarisation use like the GOES and other L band satellites.

Switching between vertical and horizontal polarisations is aheived by changeing the supply on coax from 12v to 18v as in the normal satelite TV LNB usage.

These Sband LNBs are used on the SES7 MNC / Indovision 2.5 ghz signal which is possibly the only direct brodcast satelite to use S band, availiblity is local to Indonessia
from many online shops selling DVB-Ss set top recievers and associated equipment for around the $10 dollar mark.

It works fine with an RTL-SDR requiring only an inline power injector or bias tee, the 5v bias tee output of an sdr is not suitable.

Mounted offest in a 1.8mt c band dish with the prime Cband LNB set on Telstar vantage it works fine with 100 metres of RG11 cable run to the V3 RTL-SDR 
using the software provided by this project on github. https://vksdr.com/xrit-rx
