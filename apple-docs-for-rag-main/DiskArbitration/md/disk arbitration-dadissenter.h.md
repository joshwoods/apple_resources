

- Disk Arbitration
-  DADissenter.h 

API Collection

# DADissenter.h

## Overview

See the Overview section above for header-level documentation.

## Overview

### Included Headers

- \

- \

## Topics

### Miscellaneous

func DADissenterCreate(CFAllocator?, DAReturn, CFString?) -> DADissenter

Creates a new dissenter object.

func DADissenterGetStatus(DADissenter) -> DAReturn

Obtains the return code.

func DADissenterGetStatusString(DADissenter) -> CFString?

Obtains the return code string.

### Data Types

class DADissenter

Type of a reference to DADissenter instances.

## See Also

### Reference

DADisk.h

DASession.h

DiskArbitration.h

Register for mount/unmount notifications, and block mount/unmount events.

DiskArbitration Enumerations

DiskArbitration Constants

DiskArbitration Data Types

