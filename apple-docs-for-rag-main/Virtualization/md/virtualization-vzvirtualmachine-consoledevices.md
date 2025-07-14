

- Virtualization
- VZVirtualMachine
-  consoleDevices 

Instance Property

# consoleDevices

The list of configured console devices on the VM.

macOS 13.0+

``` source
var consoleDevices: [VZConsoleDevice] { get }
```

## Discussion

Return an empty array if there are no console devices configured.

## See Also

### Configuring VM attributes at runtime

var memoryBalloonDevices: [VZMemoryBalloonDevice]

The array of devices that you use to adjust the amount of memory available to the guest system.

var networkDevices: [VZNetworkDevice]

The list of configured network devices on the VM.

var socketDevices: [VZSocketDevice]

The array of socket devices that the VM configures for use ports in the guest VM.

var directorySharingDevices: [VZDirectorySharingDevice]

The list of configured directory-sharing devices on the VM.

var usbControllers: [VZUSBController]

The list of runtime USB controller objects.

