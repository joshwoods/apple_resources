

- TabularData
- ColumnSlice
-  ColumnProtocol Implementations 

API Collection

# ColumnProtocol Implementations

## Topics

### Operators

static func + (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by adding a value to each element in a column.

static func + (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column to a value.

static func - (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by subtracting a value from each element in a column.

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

