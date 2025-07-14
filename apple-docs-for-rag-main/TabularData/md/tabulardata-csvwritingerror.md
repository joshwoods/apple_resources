

- TabularData
-  CSVWritingError 

Enumeration

# CSVWritingError

A CSV writing error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum CSVWritingError
```

## Topics

### Getting Error Information

var column: String?

The index of the column that contains the error.

var row: Int

The index of the row that contains the error.

case badEncoding(row: Int, column: String, Data)

An error that indicates CSV data contains an invalid UTF-8 byte sequence.

### Default Implementations

CustomStringConvertible Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Error
- Sendable

## See Also

### Errors

enum JSONReadingError

A JSON reading error.

enum CSVReadingError

A CSV reading error.

struct ColumnDecodingError

A column decoding error.

struct ColumnEncodingError

A column encoding error.

enum SFrameReadingError

An error when reading a Turi Create scalable data frame.

