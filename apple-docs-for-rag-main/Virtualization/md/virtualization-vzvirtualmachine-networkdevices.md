

- Virtualization
- VZVirtualMachine
-  networkDevices 

Instance Property

# networkDevices

The list of configured network devices on the VM.

macOS 12.0+

``` source
var networkDevices: [VZNetworkDevice] { get }
```

## Discussion

Returns an empty array if there are no configured network devices.

## See Also

### Configuring VM attributes at runtime

var consoleDevices: [VZConsoleDevice]

The list of configured console devices on the VM.

var memoryBalloonDevices: [VZMemoryBalloonDevice]

The array of devices that you use to adjust the amount of memory available to the guest system.

var socketDevices: [VZSocketDevice]

The array of socket devices that the VM configures for use ports in the guest VM.

var directorySharingDevices: [VZDirectorySharingDevice]

The list of configured directory-sharing devices on the VM.

var usbControllers: [VZUSBController]

The list of runtime USB controller objects.

