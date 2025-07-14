

- Virtualization
- VZGraphicsDevice
-  displays 

Instance Property

# displays

The list of graphics displays configured for this graphics device.

macOS 14.0+

``` source
var displays: [VZGraphicsDisplay] { get }
```

## Discussion

This is a list of the graphics displays configured on the graphics device configuration.

## See Also

### Related Documentation

class VZMacGraphicsDisplayConfiguration

The configuration for a Mac graphics device.

class VZVirtioGraphicsScanoutConfiguration

The configuration for a Virtio graphics device that configures the dimensions of the graphics device for a Linux VM.

