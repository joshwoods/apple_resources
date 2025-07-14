

- FSKit
-  FSDirectoryEntryPacker 

Class

# FSDirectoryEntryPacker

An object used to provide items during a directory enumeration.

macOS 15.4+

``` source
class FSDirectoryEntryPacker
```

## Overview

You use this type in your implementation of enumerateDirectory(_:startingAt:verifier:attributes:packer:replyHandler:).

Packing allows your implementation to provide information FSKit needs, including each item’s name, type, and identifier (such as an inode number). Some directory enumerations require other attributes, as indicated by the FSItem.GetAttributesRequest sent to the enumerate method.

## Topics

### Packing entries

func packEntry(name: FSFileName, itemType: FSItem.ItemType, itemID: FSItem.Identifier, nextCookie: FSDirectoryCookie, attributes: FSItem.Attributes?) -> Bool

Provides a directory entry during enumeration.

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

### Inspecting directory contents

func enumerateDirectory(FSItem, startingAt: FSDirectoryCookie, verifier: FSDirectoryVerifier, attributes: FSItem.GetAttributesRequest?, packer: FSDirectoryEntryPacker, replyHandler: (FSDirectoryVerifier, (any Error)?) -> Void)

Enumerates the contents of the given directory.

**Required**

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

struct FSDirectoryVerifier

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

struct FSDirectoryVerifier

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

