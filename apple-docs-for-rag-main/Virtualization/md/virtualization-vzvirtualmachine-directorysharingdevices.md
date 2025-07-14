

- Virtualization
- VZVirtualMachine
-  directorySharingDevices 

Instance Property

# directorySharingDevices

The list of configured directory-sharing devices on the VM.

macOS 12.0+

``` source
var directorySharingDevices: [VZDirectorySharingDevice] { get }
```

## Discussion

Returns an empty array if there are no directory sharing devices associated with this virtual machine.

## See Also

### Configuring VM attributes at runtime

var consoleDevices: [VZConsoleDevice]

The list of configured console devices on the VM.

var memoryBalloonDevices: [VZMemoryBalloonDevice]

The array of devices that you use to adjust the amount of memory available to the guest system.

var networkDevices: [VZNetworkDevice]

The list of configured network devices on the VM.

var socketDevices: [VZSocketDevice]

The array of socket devices that the VM configures for use ports in the guest VM.

var usbControllers: [VZUSBController]

The list of runtime USB controller objects.

