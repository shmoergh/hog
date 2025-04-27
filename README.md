# Hog

Fully analog two-voice monophonic synth for live performances.

![hog-4](https://github.com/user-attachments/assets/5aac2ab4-8e55-40d0-9659-4bc40b0307c7)


Details and user guide: [shmoergh.com](https://shmoergh.com/)

Latest revision: rev #3.

## Build

The HOG is a very fun but equally advanced electronics project. It's fully open source and we've put together a build guide for the brave ones who decide to build one. Let us know if you have questions and definitely share some pics of your builds (follow [Shmøergh on Instagram](https://www.instagram.com/shmoergh/)).

[Open build guide &rarr;](https://www.shmoergh.com/guides/hog-build-guide)


## BOMs

The HOG consists of 5 separate boards which you can find in the `boards` folder. Each board has it's own gerber files for JLCPCB PCB and Mouser BOMs in the board's `production` folders. The Core and Filter boards have SMD components too for which you can find JLCPCB assembly files (BOM and position) in the `production/jlcpcb` folder.


## Cloning

The MIDI2CV module uses [`pico-lib`](https://github.com/peterzimon/pico-lib) submodule. Make sure you clone
the repo like with its submodules:

```
git clone --recurse-submodules git@github.com:shmoergh/hog.git
```

## License

Shmoergh Hog © 2024

Hardware is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)

Software is licensed under [MIT](https://opensource.org/license/mit).

Font used on PCBs: https://departuremono.com

Simulations made in [CircuitJS](https://www.falstad.com/circuit/circuitjs.html)
