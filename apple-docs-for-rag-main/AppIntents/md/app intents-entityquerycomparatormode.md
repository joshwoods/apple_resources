

- App Intents
-  EntityQueryComparatorMode 

Enumeration

# EntityQueryComparatorMode

Modes that determine how to apply a query’s comparators.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
enum EntityQueryComparatorMode
```

## Topics

### Comparator modes

case and

case or

### Operators

static func == (EntityQueryComparatorMode, EntityQueryComparatorMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

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

### Searching for entities

func entities(matching: [Self.ComparatorMappingType], mode: Self.ComparatorMode, sortedBy: [EntityQuerySort&lt;Self.Entity>], limit: Int?) async throws -> Self.Result

Retrieves instances matching the supplied comparators.

**Required**

typealias Sort

typealias ComparatorMode

