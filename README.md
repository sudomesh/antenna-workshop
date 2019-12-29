
This repo contains research and materials for the [sudo mesh](https://sudomesh.org) Antenna Design Workshop.

The workshop was inspired by [this youtube video](https://www.youtube.com/watch?v=drwGvATLNaw), the availability of [the cheap N1201SA antenna analyzer](https://www.ebay.com/sch/i.html?_nkw=N1201SA) and a need for more hands-on learning experiences at our recurring [Build Your Own Internet](https://buildyourowninter.net/) workshops.

# Antenna designs

Information on viable antenna designs is in the `ANTENNA_DESIGN.md` file.

# Description

This is the description as written in the grant proposal:

Participants will cut conductive copper tape into shapes and stick it onto plain FR4 (circuitboard material). They will then get to test the resonance frequency of their improvised PCB and wire antennas using a Vector Network Analyzer and perform a rough check of antenna directionality by hooking them up to a transmitter and pointing them at different strategically placed directional receivers. We expect much testing and re-tweaking of shapes to get the resonance frequency just right.

We'll include a very brief presentation on guidelines for making different kinds of antennas and have volunteers to answer questions throughout.

This workshop won't require any prior experience and be open to all ages (under 18 to be accompanied by a parent or guardian). Everything but the copper tape and wire will be re-usable for later workshops.

For anyone interested we'll have a follow-up session for translating the designs into KiCAD and ordering them from a PCB manufacturing company.

## What are the project goals?

The main goal is to engage some of the local community in thinking about a part of our communications infrastructure that's usually invisible, and hopefully to learn something and have fun along the way. We want to convey a sense that the technologies we rely on every day for our internet connectivity are not out of reach for improvement and creative modification by individuals and small groups.

We will document the experience on our blog and wiki, including how many attendees we have and how many antenna prototypes were built and tested. We'll also provide material to help others who want to run a similar workshop.

A secondary goal is to test the viability of this method of rapid PCB antenna prototyping for e.g. open hardware projects by getting a sense of the difference between the hand-prototyped antennas and the equivalent professionally manufactured antennas.

## Who will it benefit?

This will benefit anyone local to the SF Bay Area interested in how wireless sig
nals and antennas work. Based on attendence at previous events we expect a wide 
range of experience levels from young kids to licensed HAM radio operators. 

We'll document this effort on our wiki and blog to make it easy for others to set up a similar antenna workshop, and we'll share our successes and failures so others can improve upon the experience. We expect that this method of prototyping antennas is relatively unknown and may also be of use to more seasoned eletronics engineers. We hope to provide actual numbers on the deviation between "copper tape on plain FR4" and the same design manufactured by a PCB manufacturing facility.

# FR4 material

For the PCB prototyping we need reasonable large sheets of FR4 (e.g. 1 foot squares) without any copper coating.

I got a quote from [Suzhou Zheng Sheng Insulating Materials](https://www.alibaba.com/product-detail/Yellow-Light-Green-Black-Epoxy-Resin_60564676529.html) for 12pcs 300*300*1.6mm for $26.4 + $58.6 shipping for 5 kg via DHL for a total of $85.

I found another supplier on ebay and that was even more expensive.

We can get 30pcs single-sided manufactured 300x300x1.6mm PCB from [JLBPCB.com](https://jlcpcb.com/) for ~$196 + ~$61 shipping.

It _would_ be nice to get blank PCB from a manufacturer so we can then test the difference between the same antenna design as manufactured and as prototyped with conductive tape.

# Conductive tape

We can either use cheap conductive copper tape or we can use tape that has conductive adhesive. The connection through the conductive adhesive is very likely going to seriously affect the antennas performance but it would make it easier to cut and paste rather than having to solder pieces of tape together. Another option is to use very wide conductive copper tape so we never have to connect two pieces. We'd need 12" wide tape for that to work.

Apparently you can get cheap 30 x 22.5 cm adhesive copper foil sheets for use on guitars(?) [on ebay](https://www.ebay.com/itm/Guitar-Copper-Foil-Tape-EMI-Shielding-Foil-Tape-for-Electric-Guitar-4-Sheet/202664750602). Looks like $6.51 for four sheets so if we got e.g. 70 sheets for our 35 FR4 sheets it'd cost around $120.

Or we could just buy some 6" by 10' tape for $12 that actually has a brand and is sold by a local seller [here](https://www.ebay.com/itm/Copper-Foil-Tape-6-X-10ft-EMI-Conductive-Adhesive-Ship-from-USA/152088504474).

Maybe worth it to a buy a bit of all three kinds and try it out first?

# Budget

Original budget estimate:

* N1201SA Antenna analyzer: $200
* 35 sheets of ~330x330x1.6mm FR4: ~$200 shipped
* Conductive copper shielding tape 10 cm x 15 m: ~$50 shipped
* Coax cable stripper and cimper: $100
* Antenna connectors and cable: $50
* Various off-the-shelf antennas for teardown and testing against: $200
* Drinks and snacks: $200

# Funding

This workshop was funded by a grant from [No Starch Press](https://nostarch.com/).