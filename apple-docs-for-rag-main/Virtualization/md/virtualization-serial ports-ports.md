

- Virtualization
-  Serial ports 

API Collection

# Serial ports

Configure the serial devices that you use to communicate with the guest system.

## Topics

### Configurations

class VZVirtioConsoleDeviceSerialPortConfiguration

A configuration object that requests the creation of a console device to communicate with the guest system.

class VZSerialPortConfiguration

The common configuration traits for serial port requests.

### Attachment points

class VZFileHandleSerialPortAttachment

An attachment point that allows bidirectional communication using file handles.

class VZFileSerialPortAttachment

An attachment point that writes data from the guest system to a file.

class VZSerialPortAttachment

The common behaviors for the serial attachment points of your virtual machine.

## See Also

### Devices

Audio

Configure audio devices that enable the guest operating system to perform audio playback and capture through the host’s audio devices.

Graphics

Configure a device for a guest to display its UI.

Keyboards and pointing devices

Configure devices that connect a mouse and keyboard to the guest system.

Memory

Configure a memory balloon device to change the allocated memory for the guest system.

Network

Configure the devices that connect the guest system to the network.

Randomization

Configure a device for the guest system to use to generate random numbers.

Shared directories

Configure devices that share directories from the host into the guest system.

Sockets

Configure a device that manages port-based communication with the guest system.

Storage

Configure the block-storage devices that represent the disks of the guest system.

Consoles

Configure a device that manages multiport console communication with the guest system.

Clipboard sharing

Share the pasteboard between the host and guest system.

USB Devices

