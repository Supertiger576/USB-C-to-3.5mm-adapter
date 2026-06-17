# About
A straight-forward adapter using a DAC that translates USB-C audio data to 3.5mm.  It takes in the digital USB-C sound data, and then uses the PCM2902 DAC to translate it into analog sound data that can be outputted through a 3.5mm headphone jack.  The PCM2902 DAC is wired following references from it's datasheet. 

# Use
I wanted to make this project as it would be useful for being able to listen to music on the go, without having wireless ear buds.

# Schematic:       
<img width="478" height="311" alt="image" src="https://github.com/user-attachments/assets/c489301b-c81c-4616-ae84-9a5738679234" />      
      
# PCB:      
<img width="720" height="347" alt="image" src="https://github.com/user-attachments/assets/0c03bfc6-2d72-40b3-8ab2-e6241ec7de19" />    
   
# 3D Model:    
<img width="598" height="284" alt="image" src="https://github.com/user-attachments/assets/9359bedd-0ad9-401b-bd7f-e1861f3ab530" />    

# Necessary Materials:
|Name                     |Purpose                                                                                           |Quantity|Total Cost (USD)|Link                                                                                                                      |Distributor|
|-------------------------|--------------------------------------------------------------------------------------------------|--------|----------------|--------------------------------------------------------------------------------------------------------------------------|-----------|
|PCB                      |The PCB to put the other components on                                                            |1       |2.00            |https://jlcpcb.com                                                                                                        |JLCPCB     |
|1 uf capacitors          |To connect VC... pins to GND like in the reference sheet.  I only need 6 but buying 10 is cheaper.|10      |0.49            |https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL21B105KAFNNNE/3886724                              |Digikey    |
|15 pF capacitors         |Connecting to the crystal oscillator to handle load                                               |2       |0.22            |https://www.digikey.com/en/products/detail/kemet/C0805C150J5GACTU/411110?s=N4IgTCBcDaIMIAYAcCCscCMqEClUHEBBOAFQFUACEAXQF8g|Digikey    |
|10 uf capacitor          |Capacitor to clear audio on L_out and R_out                                                       |2       |0.60            |https://www.digikey.com/en/products/detail/rubycon/50YXJ10M5X11/3562914                                                   |Digikey    |
|12 MHz Crystal Oscillator|Stable timing on the USBC                                                                         |1       |0.56            |https://www.digikey.com/en/products/detail/kyocera-avx/CX3225SB12000D0GZJC1/5995239                                       |Digikey    |
|1M ohm resistor          |Connected to the crystal oscillator                                                               |1       |0.10            |https://www.digikey.com/en/products/detail/yageo/MFR-25FBF52-1M/13714                                                     |Digikey    |
|DX07P024AJ5R1500         |The usbc plug port for my adapter                                                                 |1       |1.83            |https://www.digikey.com/en/products/detail/jae-electronics/DX07P024AJ5R1500/9169455                                       |Digikey    |
|PCM2902CDBR DAC          |The digital-to-audio converter I will use for my adapter                                          |1       |15.09           |https://www.digikey.com/en/products/detail/texas-instruments/PCM2902CDBR/2780994                                          |Digikey    |
|TRS headphone jack       |The headphone jack at one end of my converter                                                     |1       |0.88            |https://www.digikey.com/en/products/detail/same-sky-formerly-cui-devices/SJ-3523-SMT-TR/281297                            |Digikey    |
|22 ohm resistors         |To connect to D+ and D-                                                                           |2       |0.20            |https://www.digikey.com/en/products/detail/yageo/CFR-50JB-52-22R/1303                                                     |Digikey    |
|5.1k ohm resistors       |To connect to the CC and VCONN channels                                                           |2       |0.20            |https://www.digikey.com/en/products/detail/yageo/CFR-25JT-52-5K1/9098642                                                  |Digikey    |

Made with KiCad
