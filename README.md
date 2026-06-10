# Utils

Simple and useful utilities when working at the command line. Adds commands that simplify output of other commands for easy reading. Add this directory to your `$PATH` and use the commands below.

## Battery Status

Displays the current battery status to the command line. Useful for working on a laptop. Command:

```sh
battery
```

## Disks

Displays a simple, short list of the disks on a system. Uses `fdisk` and will require `sudo` permissions. Command:

```sh
disks
```

## USBs

Displays a list of the USB devices using `lsusb`. Command:

```sh
usbs
```

## ep

This is a utility for hitting endpoints. The underlying technology runs on cURL.

### Setup
Execute within `utils` directory
```sh
mkdir -p endpoints/example-endpoint
echo "curl --get -w '\n' https://catfact.ninja/fact" > endpoints/example-endpoint/example
```
and then to test it out:
```sh
ep example-endpoint example
```

## timer

Simple timer utility that uses the terminal bell as an alarm. For a 10 second timer:
```sh
timer 10
```
For a 10 minute timer
```sh
timer -m 10
```
For a 10 hour timer
```sh
timer -h 10
```

## genpdf

Generates a pdf from a markdown file. Requires weasyprint and pandoc. Assumes utils is in `$HOME/.config/utils`
```sh
genpdf input.md
```
