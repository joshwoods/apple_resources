

- TabularData
-  JSONReadingError 

Enumeration

# JSONReadingError

A JSON reading error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum JSONReadingError
```

## Topics

### Getting Error Information

case failedToParse(row: Int, column: String, type: JSONType, contents: String)

An error that occurs when a JSON value fails to parse as the specified type.

case incompatibleValues(column: String)

An error that occurs when the JSON data contains incompatible values in a column.

case unsupportedStructure

An error that occurs when the JSON structure is incompatible with a data frame.

case wrongType(row: Int, column: String, expectedType: JSONType, value: any Sendable)

An error that occurs when the JSON data contains a value of the wrong type for a type-constrained column.

### Default Implementations

CustomStringConvertible Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Error
- LocalizedError
- Sendable

## See Also

### Errors

enum CSVReadingError

A CSV reading error.

enum CSVWritingError

A CSV writing error.

struct ColumnDecodingError

A column decoding error.

struct ColumnEncodingError

A column encoding error.

enum SFrameReadingError

An error when reading a Turi Create scalable data frame.

