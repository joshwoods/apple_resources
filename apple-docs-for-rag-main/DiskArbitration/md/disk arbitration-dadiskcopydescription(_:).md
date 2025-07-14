

- Disk Arbitration
-  DADiskCopyDescription(\_:) 

Function

# DADiskCopyDescription(\_:)

Obtains the Disk Arbitration description of the specified disk.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADiskCopyDescription(_ disk: DADisk) -> CFDictionary?
```

## Parameters 

`disk`  

The DADisk for which to obtain the Disk Arbitration description.

## Return Value

The disk’s Disk Arbitration description.

## Discussion

This function will contact Disk Arbitration to acquire the latest description of the specified disk, unless this function is called on a disk object passed within the context of a registered callback, in which case the description is current as of that callback event.

The caller of this function receives a reference to the returned object. The caller also implicitly retains the object and is responsible for releasing it with CFRelease().

## See Also

### Miscellaneous

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

func DADiskGetTypeID() -> CFTypeID

Returns the type identifier of all DADisk instances.

