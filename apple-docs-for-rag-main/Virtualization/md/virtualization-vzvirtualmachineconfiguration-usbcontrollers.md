

- Virtualization
- VZVirtualMachineConfiguration
-  usbControllers 

Instance Property

# usbControllers

The list of configured USB controllers for the VM.

macOS 15.0+

``` source
var usbControllers: [VZUSBControllerConfiguration] { get set }
```

## Discussion

Use this property to attach USB controllers to the VM configuration, as in the following example:

```
// Configure and start the virtual machine.
let usbControllerConfiguration = VZXHCIControllerConfiguration()

let vmConfiguration = VZVirtualMachineConfiguration()
vmConfiguration.usbControllers = [usbControllerConfiguration]

let virtualMachine = VZVirtualMachine(configuration: vmConfiguration)
try await virtualMachine.start()
```

This property contains an empty array if the `VZVirtualMachineConfiguration` doesn’t have any configured USB controllers.

## See Also

### Related Documentation

class VZUSBControllerConfiguration

The base class for a USB controller configuration.

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

var graphicsDevices: [VZGraphicsDeviceConfiguration]

The list of graphics devices.

var keyboards: [VZKeyboardConfiguration]

The list of keyboards.

var platform: VZPlatformConfiguration

The hardware platform to use.

var pointingDevices: [VZPointingDeviceConfiguration]

The list of pointing devices.

