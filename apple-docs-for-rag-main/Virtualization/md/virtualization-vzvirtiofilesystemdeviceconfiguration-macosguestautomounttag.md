

- Virtualization
- VZVirtioFileSystemDeviceConfiguration
-  macOSGuestAutomountTag 

Type Property

# macOSGuestAutomountTag

A value that indicates that the guest needs to automount this file system device in the guest VM.

macOS 13.0+

``` source
class var macOSGuestAutomountTag: String { get }
```

## Discussion

A device configured with this tag is automatically mounted in a macOS guest.

## See Also

### Getting file system information

var share: VZDirectoryShare?

A value that defines how the host exposes resources to the guest virtual machine.

var tag: String

A label that identifies this device in the guest VM.

