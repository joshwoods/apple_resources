

- Virtualization
- VZUSBDeviceConfiguration
-  uuid 

Instance Property

# uuid

The device’s unique identifier.

macOS 15.0+

``` source
var uuid: UUID { get set }
```

**Required**

## Discussion

The framework autogenerates the device UUID.

Before restoring the VM, you need to set the device’s UUID to the UUID of the device with the attachment at the time of saving the VM’s state.

