

- FSKit
- FSItem
-  FSItem.ItemType 

Enumeration

# FSItem.ItemType

An enumeration of item types, such as file, directory, or symbolic link.

macOS 15.4+

``` source
enum ItemType
```

## Topics

### Working with item types

case file

case directory

case symlink

case fifo

case charDevice

case blockDevice

case socket

case unknown

### Working with raw values

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

### Identifying an item

enum Identifier

