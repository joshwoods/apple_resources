

- Virtualization
-  VZSharedDirectory 

Class

# VZSharedDirectory

A directory on the host that you can expose to a guest.

macOS 12.0+

``` source
class VZSharedDirectory
```

## Overview

This exposes a directory from the host file system to the guest.

## Topics

### Creating a Shared Directory

init(url: URL, readOnly: Bool)

Initialize with a host directory.

### Accessing Directory Properties

var url: URL

A file URL to a directory on the host system to expose to the guest.

var isReadOnly: Bool

A Boolean value that indicates whether the directory is read-only to the guest.

## Relationships

### Inherits From

- NSObject

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

class VZDirectoryShare

The base class for a directory share.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

