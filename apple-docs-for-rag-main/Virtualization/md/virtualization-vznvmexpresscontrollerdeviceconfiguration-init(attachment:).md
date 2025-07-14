

- Virtualization
- VZNVMExpressControllerDeviceConfiguration
-  init(attachment:) 

Initializer

# init(attachment:)

Creates a new NVM Express controller configuration with the storage device attachment you provide.

macOS 14.0+

``` source
init(attachment: VZStorageDeviceAttachment)
```

## Parameters 

`attachment`  

The storage device attachment. This defines how the virtualized device operates on the host side.

## See Also

### Related Documentation

class VZDiskImageStorageDeviceAttachment

A device that stores content in a disk image.

