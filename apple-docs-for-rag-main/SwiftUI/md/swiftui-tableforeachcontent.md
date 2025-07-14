

- SwiftUI
-  TableForEachContent 

Structure

# TableForEachContent

A type of table row content that creates table rows created by iterating over a collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
struct TableForEachContent where Data : RandomAccessCollection, Data.Element : Identifiable
```

## Overview

You don’t use this type directly. The various `Table.init(_:,...)` initializers create this type as the table’s `Rows` generic type.

To explicitly create dynamic collection-based rows, use ForEach instead.

## Relationships

### Conforms To

- TableRowContent

## See Also

### Creating rows

struct TableRow

A row that represents a data value in a table.

protocol TableRowContent

A type used to represent table rows.

struct TableHeaderRowContent

A table row that displays a single view instead of columned content.

struct TupleTableRowContent

A type of table column content that creates table rows created from a Swift tuple of table rows.

struct EmptyTableRowContent

A table row content that doesn’t produce any rows.

protocol DynamicTableRowContent

A type of table row content that generates table rows from an underlying collection of data.

struct TableRowBuilder

A result builder that creates table row content from closures.

