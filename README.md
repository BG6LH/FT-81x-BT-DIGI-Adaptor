# A PCB Design of Bluetooth DIGI Adaptor for Yaesu FT-817/818 Series transceivers



> **NOTE: This Design is still a Work in Progress. Schematic, PCB, and other stuff might change!**

## Table of Contents
- [Update](#update)
- [Background](#background)
- [Design](#design)
- [Related Efforts](#related-efforts)
- [Contributing](#contributing)
- [Maintainers](#maintainers)
- [License](#license)

## Update
Updated in 20230522
1. Add 6.2V zener for pre-conditioning before LM1117-3.3
2. Add attenuation network for Line->Mic
3. Add EMI inductor on TXD/RXD pins.
4. Removed TXD's LED.


## Background
My friend BG6JJI designed a Bluetooth DIGI adaptor working for many old style TRXs with a Bluetooth, DIGI and CAT ability. He was using a Bluetooth module named JDY-67. I am not sure which manufacturer made the JDY-67. But it's really inexpensive and really works for Bluetooth Audio, and SPP in same time.

So, I pick up an old PCB design for my FT-818. It was design for FT8 cable connecting at very beginning. However, with JDY-67, It should works for Bluetooh/DIGI/CAT. I'd measured the DATA and ACC jacks on FT-818's rear panel, And refering to the FT-817ND's Service Manual, I think the Yaesu's PCB maybe design in a 0.635mm/0.025inch grid. Under this assumption, I'd drawn a PCB that could cover most of the FT-817 rear panel, and perfectly matched all the screw holes, jacks....precisely!!! It looks like a underwear(under-bottom-hardware), right?

![have a look](./pics/FT-81x-BT-DIGI-Adaptor-PIC.jpeg)

Although FT-817/818 has been discontinued, I still love this twenty years selling product. Now, I would like to share this PCB desgin to all HAM communities, If you wanna make your design, you can make any modify from it.


## Design
This PCB was design by KiCad 7.0
In the Layer User.Drawings and User.Comments, there are some information of measurement.
In the Layer User.1~4, there are approximate FT-817/818's panel sketch for comparison.

![have a look](./pics/FT-81x-BT-DIGI-Adaptor-SCH.png)
![have a look](./pics/FT-81x-BT-DIGI-Adaptor-PCB.png)
![have a look](./pics/FT-81x-BT-DIGI-Adaptor-3D.png)

## Related Efforts
- [FT8CN for Android](https://github.com/N0BOY/FT8CN) - Run FT8 natively on Android. This app works well with our Bluetooth DIGI Adaptor.


## Contributing
With special thanks to **BG6JJI, BI1EIH***. They give me many generous advice.

Let's enjoy the FT-817's last lucky underware together!!

## Maintainers
- [@BG6LH](https://github.com/BG6LH)
- [@sgub](https://github.com/sgub)

## License

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)][cc-by-nc-sa].

[![CC BY NC SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: https://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png
