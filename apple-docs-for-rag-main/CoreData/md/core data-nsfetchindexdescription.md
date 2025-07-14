

- Core Data
-  NSFetchIndexDescription 

Class

# NSFetchIndexDescription

The description of the index.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class NSFetchIndexDescription
```

## Topics

### Creating an Index Description

init(name: String, elements: [NSFetchIndexElementDescription]?)

Creates a fetch index description using the specified name and element descriptions.

### Inspecting an Index Description

var elements: [NSFetchIndexElementDescription]

An array of fetch index element descriptions.

var entity: NSEntityDescription?

The entity description for the fetch index description.

var name: String

The name of the fetch index description.

var partialIndexPredicate: NSPredicate?

A predicate that selects rows for indexing, if the index is a partial index.

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

class NSFetchIndexElementDescription

Description of an Index Element

