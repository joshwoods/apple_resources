

- TabularData
-  ColumnEncodingError 

Structure

# ColumnEncodingError

A column encoding error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ColumnEncodingError
```

## Overview

An error bundles an EncodingError with the row and column that produces the error.

## Topics

### Creating an Encoding Error

init(columnName: String, rowIndex: Int, encodingError: EncodingError)

Creates a column encoding error.

### Getting Error Information

var columnName: String

The name of the column with the error.

var debugDescription: String

A text representation of the column encoding error suitable for debugging.

var encodingError: EncodingError

The underlying encoding error.

var rowIndex: Int

The index of the column’s element with the error.

### Default Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Error
- LocalizedError
- Sendable

## See Also

### Errors

enum JSONReadingError

A JSON reading error.

enum CSVReadingError

A CSV reading error.

enum CSVWritingError

A CSV writing error.

struct ColumnDecodingError

A column decoding error.

enum SFrameReadingError

An error when reading a Turi Create scalable data frame.

