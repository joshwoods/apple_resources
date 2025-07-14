

- Disk Arbitration
-  DADiskCopyWholeDisk(\_:) 

Function

# DADiskCopyWholeDisk(\_:)

Obtain the associated whole disk object for the specified disk.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADiskCopyWholeDisk(_ disk: DADisk) -> DADisk?
```

## Parameters 

`disk`  

The disk object.

## Return Value

The disk’s associated whole disk object.

## Discussion

The caller of this function receives a reference to the returned object. The caller also implicitly retains the object and is responsible for releasing it with CFRelease().

## See Also

### Miscellaneous

func DADiskCopyDescription(DADisk) -> CFDictionary?

Obtains the Disk Arbitration description of the specified disk.

func DADiskCopyIOMedia(DADisk) -> io_service_t

Obtains the I/O Kit media object for the specified disk.

func DADiskCreateFromBSDName(CFAllocator?, DASession, UnsafePointer&lt;CChar>) -> DADisk?

Creates a new disk object.

func DADiskCreateFromIOMedia(CFAllocator?, DASession, io_service_t) -> DADisk?

Creates a new disk object.

func DADiskCreateFromVolumePath(CFAllocator?, DASession, CFURL) -> DADisk?

Creates a new disk object.

func DADiskGetBSDName(DADisk) -> UnsafePointer&lt;CChar>?

Obtains the BSD device name for the specified disk.

func DADiskGetTypeID() -> CFTypeID

Returns the type identifier of all DADisk instances.

