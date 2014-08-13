nsplit
====

Node.js implemented split funciton for split text file in line size. You can specify the tmp dir for put temp file during split file, and output folder for put final closed file.

## Install

```
npm install nsplit -g
```

## Usage

Help page:

```
nsplit -h

Usage: node nsplit [options]

Options:
   -t, --tmp        Temp folder for puting processing file
   -o, --output     Output folder for puting done file
   -l, --line       Separate by size of lines
   -c, --callback   Execute a callback script or command when every file done
   -e, --exec       Execute a script or command
   -d, --debug      Execute debug mode
   --version        print version and exit
```


## Split sample

Full command parameters:

```
nsplit -t /tmp/temp -o /tmp/output -l 300 -e 'echo done' sample.txt
```

Simple split:

```
nsplit -o /tmp/output  sample.txt
```


