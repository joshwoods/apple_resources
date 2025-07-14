

- Virtualization
- VZStorageDeviceConfiguration
-  attachment 

Instance Property

# attachment

The attachment object that provides the underlying storage for the device.

macOS 11.0+

``` source
var attachment: VZStorageDeviceAttachment { get }
```

## Discussion

The attachment object defines which local resource on the host computer appears as a disk in the virtual machine.

