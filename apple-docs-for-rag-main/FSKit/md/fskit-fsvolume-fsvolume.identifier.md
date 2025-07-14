

- FSKit
- FSVolume
-  FSVolume.Identifier 

Class

# FSVolume.Identifier

A type that identifies a volume.

macOS 15.4+

``` source
class Identifier
```

## Overview

For most volumes, the volume identifier is the UUID identifying the volume.

Network file systems may access the same underlying volume using different authentication credentials. To handle this situation, add qualifying data to identify the specific container, as discussed in the superclass, FSEntityIdentifier.

Important

Don’t subclass this class.

## Relationships

### Inherits From

- FSEntityIdentifier

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Creating a volume

init(volumeID: FSVolume.Identifier, volumeName: FSFileName)

Creates a volume with the given identifier and name.

class FSFileName

The name of a file, expressed as a data buffer.

