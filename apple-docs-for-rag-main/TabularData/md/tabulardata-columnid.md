

- TabularData
-  ColumnID 

Structure

# ColumnID

A column identifier that stores a column’s name and the type of its elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ColumnID
```

## Topics

### Creating a Column ID

init(String, T.Type)

Creates a column identifier.

### Getting the Properties

var name: String

The name of the column the identifier represents.

### Instance Properties

var type: any Any.Type

The type of elements stored in the column the identifier represents.

### Default Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Supporting Types

enum Order

A type that represents a sort ordering.

struct FormattingOptions

A set of parameters that indicate how to present the contents of data frame or column types to a printable string.

