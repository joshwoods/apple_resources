

- Virtualization
- VZVirtualMachineConfiguration
-  graphicsDevices 

Instance Property

# graphicsDevices

The list of graphics devices.

macOS 12.0+

``` source
var graphicsDevices: [VZGraphicsDeviceConfiguration] { get set }
```

## Discussion

The default value of this property is an empty array. If your VM exposes one or more graphics devices, assign an array of VZGraphicsDeviceConfiguration objects to this property.

## See Also

### Adding devices to the VM

var consoleDevices: [VZConsoleDeviceConfiguration]

The array of console devices that you expose to the guest operating system.

var networkDevices: [VZNetworkDeviceConfiguration]

The array of network devices that you expose to the guest operating system.

var socketDevices: [VZSocketDeviceConfiguration]

The socket device that you use to implement port-based communication with the guest operating system.

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

var keyboards: [VZKeyboardConfiguration]

The list of keyboards.

var platform: VZPlatformConfiguration

The hardware platform to use.

var pointingDevices: [VZPointingDeviceConfiguration]

The list of pointing devices.

var usbControllers: [VZUSBControllerConfiguration]

The list of configured USB controllers for the VM.

