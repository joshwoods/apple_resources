

- Disk Arbitration
-  DADisk.h 

API Collection

# DADisk.h

## Overview

See the Overview section above for header-level documentation.

## Overview

### Included Headers

- \

- \

- \

## Topics

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

func DADiskGetTypeID() -> CFTypeID

Returns the type identifier of all DADisk instances.

### Data Types

class DADisk

Type of a reference to DADisk instances.

## See Also

### Reference

DADissenter.h

DASession.h

DiskArbitration.h

Register for mount/unmount notifications, and block mount/unmount events.

DiskArbitration Enumerations

DiskArbitration Constants

DiskArbitration Data Types

