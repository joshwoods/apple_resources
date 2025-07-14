

- Virtualization
-  VZSingleDirectoryShare 

Class

# VZSingleDirectoryShare

An object that defines the directory share for a single directory.

macOS 12.0+

``` source
class VZSingleDirectoryShare
```

## Overview

This directory share exposes a single directory from the host file system to the guest.

## Topics

### Creating a directory share

init(directory: VZSharedDirectory)

Creates a directory share with a directory that you specify on the host.

### Accessing directory properties

var directory: VZSharedDirectory

The directory on the host to share with the guest VM.

## Relationships

### Inherits From

- VZDirectoryShare

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZDirectorySharingDeviceConfiguration

The base class for a directory sharing device configuration.

### Directory Shares

class VZMultipleDirectoryShare

An object that describes a directory share for multiple directories.

class VZSharedDirectory

A directory on the host that you can expose to a guest.

class VZDirectoryShare

The base class for a directory share.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

