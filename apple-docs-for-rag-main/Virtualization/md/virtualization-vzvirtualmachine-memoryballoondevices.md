

- Virtualization
- VZVirtualMachine
-  memoryBalloonDevices 

Instance Property

# memoryBalloonDevices

The array of devices that you use to adjust the amount of memory available to the guest system.

macOS 11.0+

``` source
var memoryBalloonDevices: [VZMemoryBalloonDevice] { get }
```

## Discussion

If you included a VZVirtioTraditionalMemoryBalloonDeviceConfiguration object in the configuration of your VM, this property contains a corresponding VZVirtioTraditionalMemoryBalloonDevice object. Use that object to adjust the amount of memory available to the guest operating system.

If you didn’t include a memory balloon object in your configuration, this property contains an empty array.

## See Also

### Configuring VM attributes at runtime

var consoleDevices: [VZConsoleDevice]

The list of configured console devices on the VM.

var networkDevices: [VZNetworkDevice]

The list of configured network devices on the VM.

var socketDevices: [VZSocketDevice]

The array of socket devices that the VM configures for use ports in the guest VM.

var directorySharingDevices: [VZDirectorySharingDevice]

The list of configured directory-sharing devices on the VM.

var usbControllers: [VZUSBController]

The list of runtime USB controller objects.

