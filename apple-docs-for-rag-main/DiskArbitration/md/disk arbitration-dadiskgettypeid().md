

- Disk Arbitration
-  DADiskGetTypeID() 

Function

# DADiskGetTypeID()

Returns the type identifier of all DADisk instances.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADiskGetTypeID() -> CFTypeID
```

## See Also

### Miscellaneous

func DADiskCopyDescription(DADisk) -> CFDictionary?

Obtains the Disk Arbitration description of the specified disk.

func DADiskCopyIOMedia(DADisk) -> io_service_t

Obtains the I/O Kit media object for the specified disk.

func DADiskCopyWholeDisk(DADisk) -> DADisk?

Obtain the associated whole disk object for the specified disk.

func DADiskCreateFromBSDName(CFAllocator?, DASession, UnsafePointer&lt;CChar>) -> DADisk?

Creates a new disk object.

func DADiskCreateFromIOMedia(CFAllocator?, DASession, io_service_t) -> DADisk?

Creates a new disk object.

func DADiskCreateFromVolumePath(CFAllocator?, DASession, CFURL) -> DADisk?

Creates a new disk object.

func DADiskGetBSDName(DADisk) -> UnsafePointer&lt;CChar>?

Obtains the BSD device name for the specified disk.

