# node-red-contrib-atcommon
A collection of [Node-RED](http://nodered.org) nodes for Advantech IIoT platform common information.

Notice that an Advantech IIoT Platform SDK have to be installed to make this node works correctly.
Advantech IIoT Platform SDK download link is shown below:
Windows:
  https://github.com/Advantech-IIoT/Platform-SDK/tree/master/windows/bin
Linux:
  https://github.com/Advantech-IIoT/Platform-SDK/tree/master/linux/bin

## Installation
Use npm command to install this package locally in the Node-RED modules directory
```bash
npm install node-red-contrib-atcommon
```
or install it globally with the command
```bash
npm install node-red-contrib-atcommon -g
```

## Usage
Platform common Node-RED node provide one node in this package.
 - Platform

The following information can be got from `Platform` node:
 - BIOS version
 - EC version
 - OS version
 - CPU name
 - Memory available
 - Disk information

 ### Example
Please refer to [demo.json](./demo.json).  
![demoflow](./demoflow.JPG)  
 - `Platform` node sends all information once at first, and if you want `OSVer` value, input `OSVer` attribute and set it to true to get only `OSVer` value.

## Test Platform
 - Windows 10 Enterprise LTSB with node.js 6.10.1

## History
 - 1.1.5 - October 2017 : Initial Release

## License
Copyright 2017 ADVANTECH Corp. under [the Apache 2.0 license](LICENSE).