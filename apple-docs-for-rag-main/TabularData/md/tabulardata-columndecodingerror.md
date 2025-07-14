

- TabularData
-  ColumnDecodingError 

Structure

# ColumnDecodingError

A column decoding error.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ColumnDecodingError
```

## Overview

This error wraps a decoding error and includes the column name and row index where the decoding error occurs.

## Topics

### Creating a Decoding Error

init(columnName: String, rowIndex: Int, decodingError: DecodingError)

Creates a column decoding error.

### Getting Error Information

var columnName: String

The name of the column with the error.

var debugDescription: String

A text representation of the column decoding error suitable for debugging.

var decodingError: DecodingError

The underlying decoding error.

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

struct ColumnEncodingError

A column encoding error.

enum SFrameReadingError

An error when reading a Turi Create scalable data frame.

