

- Virtualization
- VZVirtioFileSystemDevice
-  tag 

Instance Property

# tag

A string that identifies the device.

macOS 12.0+

``` source
var tag: String { get }
```

## Discussion

The system presents the `tag` as a label in the guest VM that identifies this device that’s available for mounting.

## See Also

### Accessing directory properties

var share: VZDirectoryShare?

A value that defines the directory share the host exposes to the guest VM.

