

- Disk Arbitration
-  DASession.h 

API Collection

# DASession.h

## Overview

See the Overview section above for header-level documentation.

## Overview

### Included Headers

- \

## Topics

### Miscellaneous

func DASessionCreate(CFAllocator?) -> DASession?

Creates a new session.

func DASessionGetTypeID() -> CFTypeID

Returns the type identifier of all DASession instances.

func DASessionScheduleWithRunLoop(DASession, CFRunLoop, CFString)

Schedules the session on a run loop.

func DASessionSetDispatchQueue(DASession, dispatch_queue_t?)

Schedules the session on a dispatch queue.

func DASessionUnscheduleFromRunLoop(DASession, CFRunLoop, CFString)

Unschedules the session from a run loop.

### Data Types

See the Overview section above for header-level documentation.

class DASession

Type of a reference to DASession instances.

## See Also

### Reference

DADisk.h

DADissenter.h

DiskArbitration.h

Register for mount/unmount notifications, and block mount/unmount events.

DiskArbitration Enumerations

DiskArbitration Constants

DiskArbitration Data Types

