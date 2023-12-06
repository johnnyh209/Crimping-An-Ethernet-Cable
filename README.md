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

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/5846d893-8fd1-47ec-8716-64ce2fbf5fce" Width="700" />

Within the realm of twisted-pair cables, there are two types of twisted-pair cables: 

1. STP (Shielded Twisted-Pair)
2. UTP (Unshielded Twisted-Pair)

STP cables have a layer of shielding around the whole cable, and/or each pair of wires; grounding is also required. STP cables are great for environments that have a lot of interference (electrical noise). UTP cables do not have this shielding, and is much more commonly used in homes. 

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/2a0a0122-f8a5-4faa-a054-51a6c70eaaba" Width="700" />

There should be lettering on the outside of the cable that indicates what shielding is used inside. Three letters are used:

1. U = Unshielded
2. S = Braided Shielding
3. F = Foil Shielding

These letters are written in the following format:
`[Overall cable shielding] / [Individual pair shielding]TP`

For example: F/UTP = there is foil shielding around the cable, but there is no shielding around each individual pair. TP just denotes that it is a twisted-pair cable.

# What You Need

Several items will be needed to crimp an ethernet cable:

* RJ45 Crimping Tool
* Cable Stripper
* RJ45 Strain Relief Boots
* RJ45 Connector
* Cable Tester
* Ethernet Cable

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/d04356ca-beca-4ee2-a140-e869aa33591c" Width="800" />

# **Step 1.** 
Insert two RJ45 Strain Relief Boots, one on each end of the ethernet cable. With the cable stripper, make a cut on the outer sheath of the ethernet cable. It is helpful to measure the length of the RJ45 connector to the cable, add a couple millimeters, and make the cut there. Though, this is not necessary but can help eliminate the need to trim the wires later. Remove the outer sheath to expose the twisted wire pairs housed inside.

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/b2f08b23-00b9-4ba8-a680-3cf2d91f1751" Height="300" />
<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/80fbd6a5-18cd-4f29-8146-4fb8dd1749e1" Height="300" />

# **Step 2.**
For each pair of twisted wires, untwist and straighten them. Be careful of breaking off the wires while doing so.

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/cfec4282-b7cf-49d5-8a51-f273c47e66f0" Width="300" />

# **Step 3.** 
Order the wires to either the T-568A or T-568B standard. In the grand scheme of things, it doesn't matter which standard you choose. However, it is important that you choose one standard and stick to it. You should not have one end of the ethernet cable be T-568A and the other end be T-568B. This creates a crossover cable, and devices connected to each other won't be able to communicate if they are expecting a straight-through connection. T-568B is more common in the US, and that is the standard this documentation will be using.

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/fb84f727-d8c7-424c-812a-5161ff468b94" Width="500" />
<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/0b292baf-7ba7-44e1-bedd-1ede0c30e87c" Width="300" />

# **Step 4.** 
If you are using a regular RJ45 connector where the wires do not go through the other end of the connector (**not** a pass-through RJ45 connector) you should trim the length of the wires if the wires are very long. Make sure that the wires are lined up straight, and make a straight, horizontal cut. Insert the ordered wires into an RJ45 connector, making sure that the wires stay in the T-568A or T-568B order. You should also make sure to have the gold contact pins of the RJ45 connector facing you when inserting the wires. 

There are two types of RJ45 connectors (also called 8P8C for 8 positions and 8 contacts): regular and pass-through. Pass-through RJ45 connectors will allow the wires to pass through the insulated conductor holes of the connector, making it easier for you to see if the wires remain in wiring standard you have chosen. Regular RJ45 connectors does not allow the wires to go through the conductor holes.

As illustrated below, the image on the left demonstrates what a pass-through RJ45 connector will be like when inserting the wires. The image on the left, which illustrates my attempt, shows what a regular RJ45 connector will look like with the wires inserted.

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/28b20d31-d711-4cf4-9e99-9c6b1c5d7b9d" Height="500" />
<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/2245dca7-cc0a-4a6b-9440-4e549bdb07dd" Height="500" />

# **Step 5.** 
Insert the RJ45 connector, which should now have the wires inserted into it, into the RJ45 crimping tool and crimp the connector. The crimping tool should have two slots, one labeled 8P and the other 6P. These labels correlated to the number of pins that your connector has. RJ45 connectors have 8 pins, and so you will be inserting the connector into the 8P slot. Crimping will push contact pads in the connector into the wires, ensuring connection between the connector and wires and that there is a strong hold.

<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/e9cf7654-a9da-4173-ae56-c9a69515043e" Width="450" />
<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/37a6c35b-b171-4ccd-9b28-6aa2ec978f73" Width="450" />

# **Step 6.**
Repeat steps 2 - 7 for the other end of the ethernet cable.
   
<img src="https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/9894bb83-12bf-4cad-85c5-1483a68529ca" Height="500" />

# **Step 7.**
The last step is to test the ethernet cable to make sure it can successfully transmit data from one end to the other. An ethernet cable tester should have two parts, a larger main unit and a smaller remote unit. Plug one end of the cable to the main unit, and plug the other end to the remote unit. For the one used in this documentation, both the main unit and remote unit have two ports each. One is 6 pins, and the other is 8 pins on both units. Likewise with the crimper tool, we will plug the ethernet cable into the 8 pin ports. 

When you turn the test unit on after plugging in the cable, a green light will go through each number. If the light goes through each number, that means your cable is working. If some of the numbers do not light up, this can indicate that you have made a mistake during the crimping process (such as both ends not using the same ordered wiring standard). If this happens, you will have to start all over.

![output](https://github.com/johnnyh209/Crimping-An-Ethernet-Cable/assets/33064730/d4a8e1e7-1acb-4487-8ba3-0d63dc3049dc)
