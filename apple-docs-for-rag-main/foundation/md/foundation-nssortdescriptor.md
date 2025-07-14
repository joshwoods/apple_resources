

- Foundation
-  NSSortDescriptor 

Class

# NSSortDescriptor

An immutable description of how to order a collection of objects according to a property common to all the objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSSortDescriptor
```

## Overview

You construct instances of NSSortDescriptor by specifying the key path of the property to compare and the order of the sort (ascending or descending). Optionally, you can also specify a selector to use to perform the comparison, which allows you to specify other comparison selectors, such as localizedStandardCompare(_:) and localizedCaseInsensitiveCompare(_:). Sorting raises an exception if the objects don’t respond to the sort descriptor’s comparison selector.

You can use sort descriptors for the following:

- Sorting an array (an instance of NSArray or NSMutableArray — see sortedArray(using:) and sort(using:))

- Comparing two objects directly (see compare(_:to:))

- Specifying the order of objects that return from a Core Data fetch request (see sortDescriptors)

## Topics

### Creating a Sort Descriptor

init(key: String?, ascending: Bool)

Creates a sort descriptor with a specified string key path and sort order.

init(key: String?, ascending: Bool, selector: Selector?)

Creates a sort descriptor with a specified string key path, ordering, and comparison selector.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool)

Creates a sort descriptor with a specified key path and ordering.

init(key: String?, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified string key path and ordering, and a comparator block.

convenience init&lt;Root, Value>(keyPath: KeyPath&lt;Root, Value>, ascending: Bool, comparator: Comparator)

Creates a sort descriptor with a specified key path and ordering, and a comparator block.

init?(coder: NSCoder)

Creates a sort descriptor by decoding from the coder you specify.

convenience init&lt;Compared>(SortDescriptor&lt;Compared>)

Creates a sort descriptor using a sort descriptor you specify.

Deprecated

### Getting Information About a Sort Descriptor

var ascending: Bool

A Boolean value that indicates whether the receiver specifies sorting in ascending order.

var key: String?

The key that specifies the property to compare during sorting.

var keyPath: AnyKeyPath?

The key path that specifies the property to compare during sorting.

var selector: Selector?

The selector for comparing objects.

var comparator: Comparator

The comparator for the sort descriptor.

### Using Sort Descriptors

func compare(Any, to: Any) -> ComparisonResult

Returns a comparison result value that indicates the sort order of two objects.

var reversedSortDescriptor: Any

Returns a sort descriptor that reverses the sort order.

func allowEvaluation()

Forces a securely decoded sort descriptor to allow evaluation.

### Initializers

convenience init&lt;Compared>(SortDescriptor&lt;Compared>)

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
- NSSecureCoding

## See Also

### Sorting

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

enum SortOrder

The orderings that you can perform sorts with.

