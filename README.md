# Morse Code Translator
A customized device driver for Raspberry Pi 3

## Description
This repository contains a device driver of Morse Code Translator using LED working on Rasperry Pi 3 (Raspbian).

## Software Setup
* Clone this repository.
```
git clone https://github.com/masash1/robosys1.git
```
* Move to the directory and run 'make' and 'make insert' commands.
```
cd robosys1
make && make insert
```
* To remove the driver, run the commands below in the directory.
```
make remove
```
## Hardware Setup (Example)
* Connect a LED between GPIO25 and GND.
  * GPIO25: 22 pin
  * GND: 39 pin
  * The positive (longer lead) should be connected to GPIO25
* Better to add a resistance.

## Usage
* Write the words you would like to translate between 'echo' and '> /dev/myled0'.
```
echo fuck my life > /dev/myled0
```

## Demo
https://www.youtube.com/watch?v=eRkXRGBow-k&t=9s

## Reference
https://github.com/ryuichiueda/robosys2017/blob/master/07.md

## License
This repository is licensed under the GPLv3 license, see [LICENSE](./LICENSE).
