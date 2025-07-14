

- TabularData
- FilledColumn
-  ColumnProtocol Implementations 

API Collection

# ColumnProtocol Implementations

## Topics

### Operators

static func != (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type isn’t equal to a value.

static func != (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value isn’t equal to the corresponding element of a column type.

static func * (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column by a value.

static func * (Self, Self) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column type by the corresponding elements of another.

static func * (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by multiplying a value by each element in a column.

static func + (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column to a value.

static func + (Self, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column type to the corresponding elements of another.

static func + (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by adding a value to each element in a column.

static func - (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by subtracting a value from each element in a column.

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

static func - (Self, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of another.

static func == (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is equal to a value.

static func == (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is equal to the corresponding element of a column type.

static func / (Self.Element, Self) -> Column&lt;Self.Element>

Generates an integer column by dividing a value by each element in a column.

static func / (Self, Self.Element) -> Column&lt;Self.Element>

Generates a floating-point column by dividing each element in a column by a value.

static func &lt; (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is less than the corresponding element of a column type.

static func > (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is greater than a value.

static func > (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is greater than the corresponding element of a column type.

static func / (Self.Element, Self) -> Column&lt;Self.Element>

Generates a floating-point column by dividing a value by each element in a column.

static func / (Self, Self.Element) -> Column&lt;Self.Element>

Generates an integer column by dividing each element in a column by a value.

static func &lt; (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is less than a value.

static func / (Self, Self) -> Column&lt;Self.Element>

Generates a floating-point column by dividing each element in a column type by the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.Element>

Generates an integer column by dividing each element in a column type by the corresponding elements of another.

static func >= (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is greater than or equal to a value.

static func &lt;= (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is less than or equal to the corresponding element of a column type.

static func &lt;= (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is less than or equal to a value.

static func >= (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is greater than or equal to the corresponding element of a column type.

