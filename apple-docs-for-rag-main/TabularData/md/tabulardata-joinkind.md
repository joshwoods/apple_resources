

- TabularData
-  JoinKind 

Enumeration

# JoinKind

An operation type that joins two data frame types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum JoinKind
```

## Topics

### Operators

static func == (JoinKind, JoinKind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case full

A join kind that contains every row from both data frame types.

case inner

A join kind that only contains rows with matching values in both data frame types.

case left

A join kind that contains all rows from the left data frame type, and only the rows with matching values from the right data frame type.

case right

A join kind that contains all rows from the right data frame type, and only the rows with matching values from the left data frame type.

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

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a Data Frame by Joining Another Data Frame

func joined&lt;R>(R, on: String, kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type with a common column you select by name.

func joined&lt;R>(R, on: (left: String, right: String), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by name for both data frame types.

func joined&lt;R, T>(R, on: (left: ColumnID&lt;T>, right: ColumnID&lt;T>), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by identifier for both data frame types.

func joined&lt;R, T>(R, on: ColumnID&lt;T>, kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type with a common column that you select by identifier.

