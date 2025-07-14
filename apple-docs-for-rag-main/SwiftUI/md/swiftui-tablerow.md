

- SwiftUI
-  TableRow 

Structure

# TableRow

A row that represents a data value in a table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
struct TableRow where Value : Identifiable
```

## Overview

Create instances of TableRow in the closure you provide to the `rows` parameter in Table initializers that take columns and rows. The table provides the value of a row to each column of a table, which produces the cells for each row in the column.

## Topics

### Creating a row

init(Value)

Creates a table row for the given value.

## Relationships

### Conforms To

- TableRowContent

## See Also

### Creating rows

protocol TableRowContent

A type used to represent table rows.

struct TableHeaderRowContent

A table row that displays a single view instead of columned content.

struct TupleTableRowContent

A type of table column content that creates table rows created from a Swift tuple of table rows.

struct TableForEachContent

A type of table row content that creates table rows created by iterating over a collection.

struct EmptyTableRowContent

A table row content that doesn’t produce any rows.

protocol DynamicTableRowContent

A type of table row content that generates table rows from an underlying collection of data.

struct TableRowBuilder

A result builder that creates table row content from closures.

