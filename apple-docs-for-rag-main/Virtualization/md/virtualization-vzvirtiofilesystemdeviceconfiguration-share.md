

- Virtualization
- VZVirtioFileSystemDeviceConfiguration
-  share 

Instance Property

# share

A value that defines how the host exposes resources to the guest virtual machine.

macOS 12.0+

``` source
var share: VZDirectoryShare? { get set }
```

## See Also

### Getting file system information

var tag: String

A label that identifies this device in the guest VM.

class var macOSGuestAutomountTag: String

A value that indicates that the guest needs to automount this file system device in the guest VM.

