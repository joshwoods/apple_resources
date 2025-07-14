

- Virtualization
- VZVirtualMachine
-  usbControllers 

Instance Property

# usbControllers

The list of runtime USB controller objects.

macOS 15.0+

``` source
var usbControllers: [VZUSBController] { get }
```

## Discussion

Return an empty array if there isn’t a configured controller USB.

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

var directorySharingDevices: [VZDirectorySharingDevice]

The list of configured directory-sharing devices on the VM.

