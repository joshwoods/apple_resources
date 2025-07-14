

- TabularData
- Column
-  OptionalColumnProtocol Implementations 

API Collection

# OptionalColumnProtocol Implementations

## Topics

### Operators

static func * (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying a value by each element in an optional column type.

static func * (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying each element in an optional column type by the corresponding elements of another.

static func * (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying each element in an optional column by a value.

static func + (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column type to the corresponding elements of another.

static func + (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by adding a value to each element in an optional column.

static func + (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column to a value.

static func - (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting each element in an optional column from a value.

static func - (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting a value from each element in an optional column type.

static func - (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting each element in an optional column type from the corresponding elements of another.

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column by a value.

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column type by the corresponding elements of another.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing a value by each element in an optional column type.

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column by a value.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing a value by each element in an optional column type.

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column type by the corresponding elements of another.

### Instance Methods

func description(options: FormattingOptions) -> String

Generates a string description of the optional column type.

func filled(with: Self.WrappedElement) -> FilledColumn&lt;Self>

Generates a filled column by replacing missing elements with a value.

