

- SwiftUI
-  TupleTableRowContent 

Structure

# TupleTableRowContent

A type of table column content that creates table rows created from a Swift tuple of table rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@frozen
struct TupleTableRowContent where Value : Identifiable
```

## Overview

Don’t use this type directly; instead, SwiftUI uses this type as the return value from the various `buildBlock` methods in TableRowBuilder. The size of the tuple corresponds to how many columns you create in the `rows` closure you provide to the Table initializer.

## Topics

### Accessing the value

var value: T

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

struct TableForEachContent

A type of table row content that creates table rows created by iterating over a collection.

struct EmptyTableRowContent

A table row content that doesn’t produce any rows.

protocol DynamicTableRowContent

A type of table row content that generates table rows from an underlying collection of data.

struct TableRowBuilder

A result builder that creates table row content from closures.

