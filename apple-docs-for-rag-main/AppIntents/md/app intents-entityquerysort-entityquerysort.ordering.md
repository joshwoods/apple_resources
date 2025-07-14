

- App Intents
- EntityQuerySort
-  EntityQuerySort.Ordering 

Enumeration

# EntityQuerySort.Ordering

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
enum Ordering
```

## Topics

### Operators

static func == (EntityQuerySort&lt;Entity>.Ordering, EntityQuerySort&lt;Entity>.Ordering) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case ascending

case descending

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the sort order

let order: EntityQuerySort&lt;Entity>.Ordering

