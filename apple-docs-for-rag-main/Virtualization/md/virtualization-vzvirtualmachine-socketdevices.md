

- Virtualization
- VZVirtualMachine
-  socketDevices 

Instance Property

# socketDevices

The array of socket devices that the VM configures for use ports in the guest VM.

macOS 11.0+

``` source
var socketDevices: [VZSocketDevice] { get }
```

## Discussion

If you included a VZVirtioSocketDeviceConfiguration object in the configuration of your VM, this property contains a corresponding VZVirtioSocketDevice object. Use that object to configure the ports your VM makes available to the guest operating system.

If you didn’t include a socket device in your configuration, this property contains an empty array.

## See Also

### Configuring VM attributes at runtime

var consoleDevices: [VZConsoleDevice]

The list of configured console devices on the VM.

var memoryBalloonDevices: [VZMemoryBalloonDevice]

The array of devices that you use to adjust the amount of memory available to the guest system.

var networkDevices: [VZNetworkDevice]

The list of configured network devices on the VM.

var directorySharingDevices: [VZDirectorySharingDevice]

The list of configured directory-sharing devices on the VM.

var usbControllers: [VZUSBController]

The list of runtime USB controller objects.

