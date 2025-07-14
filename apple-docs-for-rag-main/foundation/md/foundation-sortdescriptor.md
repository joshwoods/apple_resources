

- Foundation
-  SortDescriptor 

Structure

# SortDescriptor

A serializable description of how to sort numerics and strings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SortDescriptor
```

## Topics

### Creating Sort Descriptors

init?(NSSortDescriptor, comparing: Compared.Type)

Creates a sort descriptor using a sort descriptor and a type that you specify.

### Inspecting Sort Descriptors

var order: SortOrder

The sort order that the sort descriptor uses to compare.

### Initializers

init(any KeyPath&lt;Compared, String?> &amp; Sendable, comparator: String.StandardComparator)

init(any KeyPath&lt;Compared, String> &amp; Sendable, comparator: String.StandardComparator)

init(any KeyPath&lt;Compared, String> &amp; Sendable, comparator: String.StandardComparator)

init(any KeyPath&lt;Compared, String?> &amp; Sendable, comparator: String.StandardComparator)

init(any KeyPath&lt;Compared, String> &amp; Sendable, comparator: String.StandardComparator, order: SortOrder)

init(any KeyPath&lt;Compared, String> &amp; Sendable, comparator: String.StandardComparator, order: SortOrder)

init(any KeyPath&lt;Compared, String?> &amp; Sendable, comparator: String.StandardComparator, order: SortOrder)

init(any KeyPath&lt;Compared, String?> &amp; Sendable, comparator: String.StandardComparator, order: SortOrder)

init(any KeyPath&lt;Compared, Double> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Float?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int8> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int32?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UUID?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt64?> &amp; Sendable, order: SortOrder)

init&lt;Value>(any KeyPath&lt;Compared, Value?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt16> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int16> &amp; Sendable, order: SortOrder)

init&lt;Value>(any KeyPath&lt;Compared, Value> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Double?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UUID> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int32> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt64> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt32?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Bool> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int64?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Date?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Bool?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt32> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Float> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt8> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int16?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Date> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt16?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, UInt8?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int?> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int64> &amp; Sendable, order: SortOrder)

init(any KeyPath&lt;Compared, Int8?> &amp; Sendable, order: SortOrder)

### Instance Properties

var keyPath: PartialKeyPath&lt;Compared>?

var stringComparator: String.StandardComparator?

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- SortComparator

## See Also

### Sorting

class NSSortDescriptor

An immutable description of how to order a collection of objects according to a property common to all the objects.

enum ComparisonResult

Constants that indicate sort order.

protocol SortComparator

A comparison algorithm for a specified type.

struct ComparableComparator

A comparator that compares types according to their conformance to the comparable protocol.

struct KeyPathComparator

A comparator that uses another sort comparator to provide the comparison of values at a key path.

enum SortOrder

The orderings that you can perform sorts with.

