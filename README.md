# x16-edit

Text editor for Commander X16

X16 Edit is a simple text editor for the Commander X16 platform inspired by GNU Nano.

Text entered by the user is stored in banked RAM (512 KB, expandable to 2 MB).

The program is designed to handle large text files with good performance. It
is not intended to be a word processor, and will support only basic text
editor functions.


# Building

The program is written in 65c02 assembly for the ca65 compiler.

Currently, there are two build targets.

The first target (the RAM version) is to be loaded as a normal program from the filesystem. It has a BASIC header, and is started with the RUN command.

The second target is a 16 KB image to be stored in one of the ROM banks (the ROM version).


# Running the RAM version

The program is tested with X16 emulator version R38.

The emulator may be downloaded from

https://www.commanderx16.com/

Run the RAM version with the following command

x16emu -sdcard sdcard.img -prg X16EDIT.PRG -run

Loading and saving files in X16 Edit require that the emulator is started with an attached sdcard.


# Running the ROM version

There are a few more steps to set up and try the ROM version.

Please see the supplemented file docs/romnotes.pdf for details.


# X16 Community

You may read more about the Commander X16 Platform on the website

https://www.commanderx16.com/
