# GK-2A-LRIT-LNA-for-L-band

Just some notes and an example of converting a cheap S band TV LNB into an L band LNA for use on on the Korean GK-2A weather satellite but also useful for any other L band linear polarisation use like the GOES and other L band satellites.

Switching between vertical and horizontal polarisations is achieved by changing the supply voltage on the coax from 12v to 14.5v for vertical and 15.5 to 18v for horizontal as in the normal satellite TV LNB usage. There is a separate RF preamp and dipole antenna for each polarity, the power circuitry and output amplifier are common to both.

These S band LNBs are used on the SES7 at 108.2E MNC / Indovision 2.5 ghz signal which is possibly the only direct broadcast satellite to use S band, availability is local to Indonesia from many online shops selling DVB-S2 set top receivers and associated equipment for around the $10 dollar mark new. An online Ali express shop has a similar lnb but more expensive and a different dipole setup and board layout.  

It works fine with an RTL-SDR requiring only an inline power injector or bias tee, the 5v bias tee output of an sdr is not suitable, 12 volts is required.

Mounted offset for 10 degrees in a 1.8mt C band dish with the prime C band LNB set on Telstar Vantage at it works fine with 100 metres of RG11 cable run to the V3 RTL-SDR using the software provided by this LRIT project on github. https://vksdr.com/xrit-rx



There are 2 steps in the full conversion, modify the pcb into an L band dual polarity LNA, preferably but optionally modify the dipoles in the feed from 2.5 gigs to 1.7 gigs. Both with care are easy to do.

You need about 15cm of mini teflon coax, for the pcb and about 3x4 cm of copper or brass shim or plain pcb for the dipoles.

The pcb only requires 2 tracks cutting, one at the input to the S band filter the other at the coupling capacitor input to the output amplifier, this mod bypasses the filters and mixer stage. Remove the DRO cavity, this will require a small spline driver but any thing that fits is ok. The dro bead can left but is better removed for access, only best left if you might want to restore the mixer in the future. Then install the coax jumper attaching the screen at both ends first and prepare the inners to sit touching the pretinned tracks. 

A few pointers:

- Keep your fingers off the board, especially the input stages for ESD safety!

- Work slowly and carefully.

- Carefully remove any pcb laquer on the solder points before tinning them and soldering the coax.

- Attach the coax outer shield before soldering the inner to avoid any force on the tiny tracks, be quick to avoid de-laminating them.

- A tiny zero ohm chip component circled in red can removed to avoid cutting the track but don't plan on putting it back.

- A suitable 15 cm scrap of mini teflon coax can often be found in an old wifi router antenna or inside if it has 2 tnc connectors like the Dlink WRT54 devices.

Refer to the images for details.

Before modifying the dipoles, check if you can get signal. This should confirm success with the pcb mod. If you get enough at your location with your dish for reliable reception you have the option of not modifying the feed dipoles.

Extending them will make a worth while difference but you must get through 2 silicon seals to lever the front off being carefull not to break it. The front is held on by snapping over a ridge on the casting, there is a bead of silicon that can be cut out and removed to get a prise tool in. There is a second seal between the back of the cover and the lip of the casting, just apply steady pressure levering against the ridge working your way around to break it free. This is difficult and the risk of too much too quick which  might break the plastic which will deform a bit at the beginning of this process.

Take ESD precautions by putting a clip lead to the casting and then to the opposite end of the dipole to short it out before soldering, remove it in the reverse manner before moving to the next one. repeat 4 times.

Over all length should be about 88mm, you can use copper or brass strip, some circuit board, flatten out a scrap of copper tube about 5 mm wide. Mounting the extensions standing on edge has the effect of bring the dipoles forward from the back of the feed to suit the longer wavelength, avoid contact with the screw heads.

again refer to the image for details.

After testing again cleanup the old silicon and replace both when putting the cover on. Ensure by filling the gap water runs off as its installed face down.

The final result should be like the image lnb_gk-2a.png
