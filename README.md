# Crimping An Ethernet Cable

This is a documentation on crimping an ethernet cable. 

# Cat (Category)
Ethernet cables are generally divided by their `Cat` label, otherwise short for `category`. `Cat` is usually followed by a number, indicating the particular cable's version number. The most common categories in use today, from my experience, are:

1. Cat5
2. Cat5e
3. Cat6
4. Cat6a

Generally, the higher the version number, the faster the [transmission] speed and the more bandwidth the ethernet cable is capable of handling. The speed and bandwidth are summarized below. The speed will be denoted in the `Ethernet Standard` column seen in the form of `1000BASE-T` or `10GBASE-T`. The numbers, 1000 or 10, refers to the transmission speed of the cable (1000Mbps or 10Gbps respectively). BASE means that baseband technology is used for signal transmission, meaning the signal is not modulated (or changed). T means that the cable is a twisted-pair cable. 

| Category      | Ethernet Standard |  Bandwidth |
| :-------------: | :-------------: | :------------: |
| Cat5  | 1000BASE-T  | 100MHz |
| Cat5e  | 1000BASE-T  | 10MHz |
| Cat6  | 10GBASE-T*  | 250MHz |
| Cat6a  | 10GBASE-T  | 500MHz |

*Though I listed Cat6 as 10G, that comes in the cost of having a shorter cable length. 10G is possible up to a cable length of 37-55 meters.

# Twisted-Pair Cabling
Ethernet cables are most commonly twisted-pair cables. This means that the wires inside of the cable (a total of 8 wires) are twisted in groups of 2 for a total of 4 pairs. Refer to the image below:

![Twisted-Pair Cable](https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/5846d893-8fd1-47ec-8716-64ce2fbf5fce)

Within the realm of twisted-pair cables, there are two types of twisted-pair cables: 

1. STP (Shielded Twisted-Pair)
2. UTP (Unshielded Twisted-Pair)

STP cables have a layer of shielding around the whole cable, and/or each pair of wires; grounding is also required. STP cables are great for environments that have a lot of interference (electrical noise). UTP cables do not have this shielding, and is much more commonly used in homes. 

![STP and UTP Cables](https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/2a0a0122-f8a5-4faa-a054-51a6c70eaaba)

There should be lettering on the outside of the cable that indicates what shielding is used inside. Three letters are used:

1. U = Unshielded
2. S = Braided Shielding
3. F = Foil Shielding

These letters are written in the following format:
`[Overall cable shielding] / [Individual pair shielding]TP`

For example: F/UTP = there is foil shielding around the cable, but there is no shielding around each individual pair. TP just denotes that it is a twisted-pair cable.

# Crimping Ethernet Cable

Several items will be needed to crimp an ethernet cable:

* RJ45 Crimping Tool
* Cable Stripper
* RJ45 Strain Relief Boots
* RJ45 Connector
* Cable Tester
* Ethernet Cable

![Tools](https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/d04356ca-beca-4ee2-a140-e869aa33591c)

1. Insert two RJ45 Strain Relief Boots, one on each end of the ethernet cable.
2. With the cable stripper, make a cut on the outer sheath of the ethernet cable. It is helpful to measure the length of the RJ45 connector to the cable, add a couple millimeters, and make the cut there. Though, this is not necessary but can help eliminate the need to trim the wires later. Remove the outer sheath to expose the twisted wire pairs housed inside.
3. For each pair of twisted wires, untwist and straighten them. Be careful of breaking off the wires while doing so.
4. Order the wires to either the T-568A or T-568B standard. In the grand scheme of things, it doesn't matter which standard you choose. However, it is important that you choose one standard and stick to it. You should not have one end of the ethernet cable be T-568A and the other end be T-568B. This creates a crossover cable, and devices connected to each other won't be able to communicate if they are expecting a straight-through connection. T-568B is more common in the US, and that is the standard this documentation will be using.
5. If you made a huge cut when stripping the outer sheath of the ethernet cable, you should trim the length of the wires. Make sure that the wires are lined up straight, and make a straight, horizontal cut.
6. Insert the ordered wires into an RJ45 connector, making sure that the wires stay in the T-568A or T-568B order. You should also make sure to have the gold contact pins of the RJ45 connector facing you when inserting the wires. There are two types of RJ45 connectors (also called 8P8C for 8 positions and 8 contacts): regular and pass-through. Pass-through RJ45 connectors will allow the wires to pass through the insulated conductor holes of the connector, making it easier for you to see if the wires remain in wiring standard you have chosen. Regular RJ45 connectors does not allow the wires to go through the conductor holes.
7.  Insert the RJ45 connector, which should now have the wires inserted into it, into the RJ45 crimping tool and crimp the connector.

https://www.digitaltrends.com/computing/different-types-of-ethernet-cables-explained/
https://docs.seattlecommunitynetwork.org/learn/cable-crimping.html
https://www.truecable.com/blogs/cable-academy/how-to-choose-the-right-cable
https://www.truecable.com/blogs/cable-academy/ethernet-cable-lingo
