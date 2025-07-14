

- Create ML
- MLDataTable
-  MLDataTable.JoinType 

Enumeration

# MLDataTable.JoinType

Join types available for MLDataTable join operations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
enum JoinType
```

## Topics

### Selecting a joining operation

case inner

An operation that joins the rows of the data tables whose values match exactly.

case left

An operation that is the union between an inner join and the remaining rows from the original data table.

case right

An operation that is the union between an inner join and the remaining rows from the secondary data table.

case outer

An operation that is the union between a left join and a right join.

### Describing a joining operation

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing joining operations

static func == (MLDataTable.JoinType, MLDataTable.JoinType) -> Bool

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

### Merging Data Tables

func join(with: MLDataTable, on: String..., type: MLDataTable.JoinType) -> MLDataTable

Creates a new data table by merging two data tables by the given columns.

