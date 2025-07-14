

- Create ML
- MLDataTable
-  MLDataTable.PackType 

Enumeration

# MLDataTable.PackType

The storage operations for combining multiple columns into one.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
enum PackType
```

## Topics

### Selecting a packing operation

case sequence

A packing type that combines the values of several columns into a sequence type.

case dictionary

A packing type that combines the values of several columns into a dictionary type.

### Describing a packing operation

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing packing operations

static func == (MLDataTable.PackType, MLDataTable.PackType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Compacting Columns

func pack(columnsNamed: String..., to: String, type: MLDataTable.PackType, filling: MLDataValue) -> MLDataTable

Creates a new data table with an additional column that contains the combined values of the given columns.

