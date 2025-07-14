

- Virtualization
-  VZMultipleDirectoryShare 

Class

# VZMultipleDirectoryShare

An object that describes a directory share for multiple directories.

macOS 12.0+

``` source
class VZMultipleDirectoryShare
```

## Overview

This directory share exposes multiple directories from the host file system to the guest VM.

## Topics

### Creating a directory share

convenience init()

Initializes the directory share with an empty set of directories.

init(directories: [String : VZSharedDirectory])

Creates the directory share with a set of directories on the host.

### Accessing the shared directories

var directories: [String : VZSharedDirectory]

The directories on the host to expose to the guest.

### Directory name utility methods

class func canonicalizedName(from: String) -> String?

Transforms a string to be a valid directory name.

class func validateName(String) throws

Check if a name is a valid directory name.

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

class VZSingleDirectoryShare

An object that defines the directory share for a single directory.

class VZSharedDirectory

A directory on the host that you can expose to a guest.

class VZDirectoryShare

The base class for a directory share.

class VZLinuxRosettaDirectoryShare

The Linux directory share for Rosetta.

