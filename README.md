# GK-2A-LRIT-LNA-for-L-band

Just some notes and an example of converting a cheap S band TV LNB into an L band LNA for use on on the Korean GK-2A weather satellite but also useful for any other L band linear polarisation use like the GOES and other L band satellites.

Switching between vertical and horizontal polarisations is achieved by changing the supply voltage on the coax from 12v to 14.5v for vertical and 15.5 to 18v for horizontal as in the normal satellite TV LNB usage. The is a separate Rf preamp and dipole antenna for each polarity, the power circuitry and output amplifier are common to both.

These S band LNBs are used on the SES7 at 108.2E MNC / Indovision 2.5 ghz signal which is possibly the only direct broadcast satellite to use S band, availability is local to Indonesia from many online shops selling DVB-S2 set top receivers and associated equipment for around the $10 dollar mark.

It works fine with an RTL-SDR requiring only an inline power injector or bias tee, the 5v bias tee output of an sdr is not suitable.

Mounted offset in a 1.8mt C band dish with the prime C band LNB set on Telstar Vantage at it works fine with 100 metres of RG11 cable run to the V3 RTL-SDR using the software provided by this LRIT project on github. https://vksdr.com/xrit-rx

