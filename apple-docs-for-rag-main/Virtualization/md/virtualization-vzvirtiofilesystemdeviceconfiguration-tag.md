

- Virtualization
- VZVirtioFileSystemDeviceConfiguration
-  tag 

Instance Property

# tag

A label that identifies this device in the guest VM.

macOS 12.0+

``` source
var tag: String { get set }
```

## See Also

### Getting file system information

var share: VZDirectoryShare?

A value that defines how the host exposes resources to the guest virtual machine.

class var macOSGuestAutomountTag: String

A value that indicates that the guest needs to automount this file system device in the guest VM.

