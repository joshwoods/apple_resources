

- TabularData
-  Order 

Enumeration

# Order

A type that represents a sort ordering.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Order
```

## Topics

### Getting the Properties

case ascending

A sort ordering that starts with the lowest value and monotonically proceeds to higher values.

case descending

A sort ordering that starts with the highest value and monotonically proceeds to lower values.

func areOrdered&lt;T>(T, T) -> Bool

Returns a Boolean that indicates whether the comparable types match the order’s state.

### Operators

static func == (Order, Order) -> Bool

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

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Supporting Types

struct ColumnID

A column identifier that stores a column’s name and the type of its elements.

struct FormattingOptions

A set of parameters that indicate how to present the contents of data frame or column types to a printable string.

