

- FSKit
-  FSDirectoryVerifier 

Structure

# FSDirectoryVerifier

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

macOS 15.4+

``` source
struct FSDirectoryVerifier
```

## Overview

Your implementation of enumerateDirectory(_:startingAt:verifier:attributes:packer:replyHandler:) defines the semantics of this value; it’s opaque to FSKit.

A tool to detect whether the directory contents changed since the last call to enumerate a directory.

Your implementation of enumerateDirectory(_:startingAt:verifier:attributes:packer:replyHandler:) defines the semantics of this value; it’s opaque to FSKit.

## Topics

### Initializing a verifier

init(UInt64)

init(rawValue: UInt64)

### Using defined verifier values

static let initial: FSDirectoryVerifier

The constant initial value for the directory-enumeration verifier.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting directory contents

func enumerateDirectory(FSItem, startingAt: FSDirectoryCookie, verifier: FSDirectoryVerifier, attributes: FSItem.GetAttributesRequest?, packer: FSDirectoryEntryPacker, replyHandler: (FSDirectoryVerifier, (any Error)?) -> Void)

Enumerates the contents of the given directory.

**Required**

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

struct FSDirectoryCookie

A value that indicates a location in a directory from which to enumerate.

class FSDirectoryEntryPacker

An object used to provide items during a directory enumeration.

