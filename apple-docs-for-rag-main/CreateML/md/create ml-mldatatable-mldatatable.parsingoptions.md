

- Create ML
- MLDataTable
-  MLDataTable.ParsingOptions 

Structure

# MLDataTable.ParsingOptions

The options for parsing a comma-separated values (CSV) file into a data table for a machine learning model.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct ParsingOptions
```

## Overview

Use `ParsingOptions` only when importing a CSV file with init(contentsOf:options:), especially if your CSV file has special formatting or your data table only needs to import specific rows or columns.

## Topics

### Creating the CSV parsing options

init(containsHeader: Bool, delimiter: String, comment: String, escape: String, doubleQuote: Bool, quote: String, skipInitialSpaces: Bool, missingValues: [String], lineTerminator: String, selectColumns: [String]?, maxRows: Int?, skipRows: Int)

Creates CSV parsing options.

### Specifying the CSV file format

var containsHeader: Bool

A Boolean value indicating whether an input CSV file contains a header.

var delimiter: String

The character that separates the data fields in a CSV file.

var lineTerminator: String

The character that represents the end of a line in a CSV file.

### Handling special characters

var escape: String

The character that marks a C escape sequence in a CSV file.

var quote: String

The character that represents a quote (`"`) in a CSV file.

var doubleQuote: Bool

A Boolean value indicating whether two consecutive quotes (`""`) represent a single quote (`"`) in a CSV file.

### Ignoring CSV components

var skipRows: Int

The number of starting rows to skip from the start of a CSV file.

var skipInitialSpaces: Bool

A Boolean value indicating whether to ignore leading spaces of a data field.

var comment: String

The character that marks the beginning of a comment, or text to ignore, in a CSV file.

### Limiting rows and columns

var maxRows: Int?

The maximum number of rows to import form a CSV file; otherwise `nil` to import all rows.

var selectColumns: [String]?

The list of column names to import from a CSV file; otherwise `nil` to import all columns.

### Representing missing values

var missingValues: [String]

A list of strings that represent missing values in a CSV file.

## Relationships

### Conforms To

- Sendable

