
This is a collection of antenna designs that could be interesting for the upcoming sudo mesh Antenna Design Workshop.

For the workshop we're mostly interested in:

* 902.3 - 914.9 MHz for LoRa
* 2412 - 2462 MHz for WiFi and bluetooth
* 2500 - 2700 MHz for channel B41 used by Spring for 4G LTE

Our antenna analyzer can't measure above 2700 MHz, but we can do some cruder measurements for:

* 5180 - 5825 MHz for WiFi

Especially the following non-DFS frequencies:

* 5180 - 5240 MHz
* 5745 - 5825 MHz

# PCB antennas

A wide variety, including yagi, log-periodic, patch and ultra wide band, are available for purchase at reasonable prices via [WA5VJB](https://wa5vjb.com/) and they have datasheets but the designs aren't open.

## Variations in PCB material

There is some good info on how much changes in dielectric constant and board thickness affects PCB antenna designs in this [Silicon Labs application note on Inverted F antennas](https://www.silabs.com/documents/public/application-notes/an1088-designing-with-pcb-antenna.pdf) (see page 9).

This data shows that the frequency where the antennas has its maximum gain is shifted by over 10 MHz by varying board thickness by 3 mils (0.0762 mm) and by around 20 Mhz by varying the dielectric constant by 0.25.

Here are the specs from a few different PCB manufacturers:

* [Seeed Studio](http://support.seeedstudio.com/knowledgebase/articles/447362-fusion-pcb-specification): +- 10% thickness, 4.2 - 4.7 dielectric constant
* [OSH Park](https://docs.oshpark.com/services/two-layer/): ? thickness, dielectric not specified higher than 100 MHz and no variance
* [JLBPCB](https://jlcpcb.com/capabilities/Capabilities): +- 10% thickness, no dielectric variance specified

It's unclear if the Seeed Studio variance in dielectric constant is from board to board or based on variations in frequency.

Based on that we can expect the frequency of an Inverted F antenna in the ~2.4 GHz band on 1.6 mm PCB to vary by:

* Seeed Studio: ~40 MHz from thickness and ~40 Mhz from dielectric constant variance
* OSH Park: ?
* JLBPCB: ~40 MHz from thickness + unknown amount from dielectric constant variance

## F antenna

These are fairly common on consumer hardware for 2.4 and 5.8 GHz. They are pretty much omnidirectional.

Some info on [The Dropout's Guide to PCB Trace Antenna Design](https://colinkarpfinger.com/blog/2010/the-dropouts-guide-to-antenna-design/) and this [Silicon Labs application note on Inverted F antennas](https://www.silabs.com/documents/public/application-notes/an1088-designing-with-pcb-antenna.pdf).

> Another variation is the meandered inverted-F antenna (MIFA). This antenna is very useful when there is a small amount of available board space. The long leg of the antenna can be meandered to reduce its footprint while still using the required conductor length. This antenna is the smallest inverted-F antenna solution for applications requiring wireless communication at 2.4 GHz. (from [Altium](https://resources.altium.com/pcb-design-blog/build-and-design-an-inverted-f-antenna-directly-on-your-pcb))

Here's an [interesting looking patent](https://patents.google.com/patent/US20030206136) that was abandoned in late 2019.

# Antennas made of bent wire

## Yagi

ToDo

Apprently the bandwidth correlates with the thickness of the waveguides?

## Moxon antenna

* [wikipedia article](https://en.wikipedia.org/wiki/Moxon_antenna)

Basically a very simple two-element yagi. Can get up to 9.7 dBi gain at 28 MHz. Not sure if more or less at higher frequencies.

The main website about them with a calculator is offline but [archive.org has a copy](https://web.archive.org/web/20180205011022/http://www.moxonantennaproject.com/design.htm).

Here's a [3D print + copper wire version](https://pinshape.com/items/26715-3d-printed-12-ghz-moxon-antenna-for-video-receiver).