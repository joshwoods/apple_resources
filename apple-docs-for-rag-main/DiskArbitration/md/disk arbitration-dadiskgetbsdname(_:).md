

- Disk Arbitration
-  DADiskGetBSDName(\_:) 

Function

# DADiskGetBSDName(\_:)

Obtains the BSD device name for the specified disk.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADiskGetBSDName(_ disk: DADisk) -> UnsafePointer?
```

## Parameters 

`disk`  

The DADisk for which to obtain the BSD device name.

## Return Value

The disk’s BSD device name.

## Discussion

The BSD device name can be used with opendev() to open the BSD device.

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

func DADiskGetTypeID() -> CFTypeID

Returns the type identifier of all DADisk instances.

