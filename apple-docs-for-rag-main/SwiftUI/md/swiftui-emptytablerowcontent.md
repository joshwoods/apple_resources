

- SwiftUI
-  EmptyTableRowContent 

Structure

# EmptyTableRowContent

A table row content that doesn’t produce any rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct EmptyTableRowContent where Value : Identifiable
```

## Overview

You will rarely, if ever, need to create an `EmptyTableRowContent` directly. Instead, `EmptyTableRowContent` represents the absence of a row.

## Relationships

### Conforms To

- Copyable
- TableRowContent

  Conforms when `Value` conforms to `Identifiable`.

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

struct TableForEachContent

A type of table row content that creates table rows created by iterating over a collection.

protocol DynamicTableRowContent

A type of table row content that generates table rows from an underlying collection of data.

struct TableRowBuilder

A result builder that creates table row content from closures.

