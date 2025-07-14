

- TabularData
-  AnyColumnSlice 

Structure

# AnyColumnSlice

A type-erased column slice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AnyColumnSlice
```

## Topics

### Inspecting a Type-Erased Column Slice

var name: String

The name of the slice’s parent column.

var count: Int

The number of elements in the column slice.

var missingCount: Int

The number of missing elements in the column slice.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

func isNil(at: Int) -> Bool

Returns a Boolean that indicates whether the element at the index is missing.

### Converting to a Typed Column Slice

func assumingType&lt;T>(T.Type) -> DiscontiguousColumnSlice&lt;T>

Returns a slice of the underlying typed column.

### Accessing Elements

subscript(Int) -> Any?

Accesses an element at an index.

subscript(Range&lt;Int>) -> AnyColumnSlice

Accesses a contiguous range of elements.

### Creating a Slice of Unique Elements

func distinct() -> AnyColumnSlice

Generates a column slice that contains unique elements.

### Summarizing a Column Slice

func summary() -> AnyCategoricalSummary

Generates a categorical summary of the column slice’s elements.

### Describing a Column Slice

var description: String

A text representation of the column slice.

var debugDescription: String

A text representation of the column slice suitable for debugging.

var customMirror: Mirror

A mirror that reflects the column slice.

### Comparing Two Column Slices

static func == (AnyColumnSlice, AnyColumnSlice) -> Bool

Returns a Boolean that indicates whether the column slices are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Hashing a Column Slice

func hash(into: inout Hasher)

Hashes the essential components of the column slice by feeding them into a hasher.

### Instance Properties

var hashValue: Int

The hash value.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AnyColumnProtocol
- BidirectionalCollection
- Collection
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- MutableCollection
- RandomAccessCollection
- Sequence

## See Also

### Type-Erased Columns

struct AnyColumn

A type-erased column.

protocol AnyColumnProtocol

A type that represents a type-erased column.

protocol AnyColumnPrototype

A prototype that creates type-erased columns.

