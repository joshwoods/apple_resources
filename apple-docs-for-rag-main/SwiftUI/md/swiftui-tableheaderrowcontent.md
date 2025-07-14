

- SwiftUI
-  TableHeaderRowContent 

Structure

# TableHeaderRowContent

A table row that displays a single view instead of columned content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct TableHeaderRowContent where Value : Identifiable, Content : View
```

## Overview

You do not create this type directly. The framework creates it on your behalf.

## Relationships

### Conforms To

- TableRowContent

## See Also

### Creating rows

struct TableRow

A row that represents a data value in a table.

protocol TableRowContent

A type used to represent table rows.

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

