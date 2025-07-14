

- Disk Arbitration
-  DADiskCreateFromIOMedia(\_:\_:\_:) 

Function

# DADiskCreateFromIOMedia(\_:\_:\_:)

Creates a new disk object.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADiskCreateFromIOMedia(
    _ allocator: CFAllocator?,
    _ session: DASession,
    _ media: io_service_t
) -> DADisk?
```

## Parameters 

`allocator`  

The allocator object to be used to allocate memory.

`session`  

The DASession in which to contact Disk Arbitration.

`media`  

The I/O Kit media object.

## Return Value

A reference to a new DADisk.

## Discussion

The caller of this function receives a reference to the returned object. The caller also implicitly retains the object and is responsible for releasing it with CFRelease().

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

func DADiskCreateFromVolumePath(CFAllocator?, DASession, CFURL) -> DADisk?

Creates a new disk object.

func DADiskGetBSDName(DADisk) -> UnsafePointer&lt;CChar>?

Obtains the BSD device name for the specified disk.

func DADiskGetTypeID() -> CFTypeID

Returns the type identifier of all DADisk instances.

