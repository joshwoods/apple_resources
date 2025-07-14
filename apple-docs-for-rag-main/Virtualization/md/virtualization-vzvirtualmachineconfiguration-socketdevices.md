

- Virtualization
- VZVirtualMachineConfiguration
-  socketDevices 

Instance Property

# socketDevices

The socket device that you use to implement port-based communication with the guest operating system.

macOS 11.0+

``` source
var socketDevices: [VZSocketDeviceConfiguration] { get set }
```

## Discussion

The default value of this property is an empty array. If your VM supports port-based communication with sockets, create a single VZVirtioSocketDeviceConfiguration object, add it to an array, and assign it to this property. After initializing the virtual machine, use the object in its socketDevices property to configure the port information and handlers.

## See Also

### Adding devices to the VM

var consoleDevices: [VZConsoleDeviceConfiguration]

The array of console devices that you expose to the guest operating system.

var networkDevices: [VZNetworkDeviceConfiguration]

The array of network devices that you expose to the guest operating system.

var serialPorts: [VZSerialPortConfiguration]

The array of serial ports that you expose to the guest operating system.

var storageDevices: [VZStorageDeviceConfiguration]

The array of storage devices that you expose to the guest operating system.

var entropyDevices: [VZEntropyDeviceConfiguration]

The array of randomization devices that you expose to the guest operating system.

var audioDevices: [VZAudioDeviceConfiguration]

The list of audio devices.

var directorySharingDevices: [VZDirectorySharingDeviceConfiguration]

The list of directory sharing devices.

var graphicsDevices: [VZGraphicsDeviceConfiguration]

The list of graphics devices.

var keyboards: [VZKeyboardConfiguration]

The list of keyboards.

var platform: VZPlatformConfiguration

The hardware platform to use.

var pointingDevices: [VZPointingDeviceConfiguration]

The list of pointing devices.

var usbControllers: [VZUSBControllerConfiguration]

The list of configured USB controllers for the VM.

