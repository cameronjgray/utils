# Utils

Simply and useful utilities when working at the command line. Adds commands that simplify output of other commands for easy reading. Add this directory to your `$PATH` and use the commands below.

## Battery Status

Displays the current battery status to the command line. Useful for working on a laptop. Command:

```sh
$ battery
```

## Disks

Displays a simple, short list of the disks on a system. Uses `fdisk` and will require `sudo` permissions. Command:

```sh
$ disks
```

## USBs

Displays a list of the USB devices using `lsusb`. Command:

```sh
$ usbs
```
