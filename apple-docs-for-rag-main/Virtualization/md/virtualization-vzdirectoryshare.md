

- Virtualization
-  VZDirectoryShare 

Class

# VZDirectoryShare

The base class for a directory share.

macOS 12.0+

``` source
class VZDirectoryShare
```

## Overview

A directory share defines how the system exposes host directories to a guest VM.

Don’t instantiate `VZDirectoryShare` directly, use one of its subclasses such as VZSingleDirectoryShare or VZMultipleDirectoryShare instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZLinuxRosettaDirectoryShare
- VZMultipleDirectoryShare
- VZSingleDirectoryShare

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Directory Shares

class VZMultipleDirectoryShare

An object that describes a directory share for multiple directories.

class VZSingleDirectoryShare

An object that defines the directory share for a single directory.

class VZSharedDirectory

A directory on the host that you can expose to a guest.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

