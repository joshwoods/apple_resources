

- Foundation
-  SortOrder 

Enumeration

# SortOrder

The orderings that you can perform sorts with.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum SortOrder
```

## Topics

### Using Sort Orders

case forward

The ordering that places the first item before the second when comparing two items using an ascending order.

case reverse

The ordering that places the first item after the second when comparing two items using an ascending order.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Sorting

class NSSortDescriptor

An immutable description of how to order a collection of objects according to a property common to all the objects.

enum ComparisonResult

Constants that indicate sort order.

struct SortDescriptor

A serializable description of how to sort numerics and strings.

protocol SortComparator

A comparison algorithm for a specified type.

struct ComparableComparator

A comparator that compares types according to their conformance to the comparable protocol.

struct KeyPathComparator

A comparator that uses another sort comparator to provide the comparison of values at a key path.

