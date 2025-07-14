

- Virtualization
- VZVirtioFileSystemDevice
-  share 

Instance Property

# share

A value that defines the directory share the host exposes to the guest VM.

macOS 12.0+

``` source
var share: VZDirectoryShare? { get set }
```

## See Also

### Related Documentation

class VZSingleDirectoryShare

An object that defines the directory share for a single directory.

class VZMultipleDirectoryShare

An object that describes a directory share for multiple directories.

### Accessing directory properties

var tag: String

A string that identifies the device.

