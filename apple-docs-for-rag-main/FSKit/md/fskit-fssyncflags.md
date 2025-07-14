

- FSKit
-  FSSyncFlags 

Enumeration

# FSSyncFlags

Behavior flags for use with synchronization calls.

macOS 15.4+

``` source
enum FSSyncFlags
```

## Overview

These values are based on flags defined in `mount.h`. Since there are system-defined flags that are valid in the kernel but not in FSKit, this type defines its members as options rather than use an enumeration.

## Topics

### Declaring synchronization behaviors

case wait

A flag for synchronized I/O with file-integrity completion.

case noWait

A flag for synchronized I/O that starts I/O but doesn’t wait for it.

case dWait

A flag for synchronized I/O with data-integrity completion.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Synchronizing with a resource

func synchronize(flags: FSSyncFlags, replyHandler: ((any Error)?) -> Void)

Synchronizes the volume with its underlying resource.

**Required**

