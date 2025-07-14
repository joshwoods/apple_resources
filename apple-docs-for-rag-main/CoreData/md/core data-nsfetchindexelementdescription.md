

- Core Data
-  NSFetchIndexElementDescription 

Class

# NSFetchIndexElementDescription

Description of an Index Element

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class NSFetchIndexElementDescription
```

## Topics

### Creating an Index Element Description

init(property: NSPropertyDescription, collationType: NSFetchIndexElementType)

Creates an index element description using the specified property description and collation type.

### Inspecting an Index Element Description

var collationType: NSFetchIndexElementType

The type of collation that the index element uses, either binary or R-tree.

var indexDescription: NSFetchIndexDescription?

var isAscending: Bool

A Boolean value that controls whether an index that supports direction is an ascending or descending index.

var property: NSPropertyDescription?

A property description.

var propertyName: String?

The specified name in the property description.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Working with indexes

enum NSFetchIndexElementType

Defines the possible types of index elements.

class NSFetchIndexDescription

The description of the index.

