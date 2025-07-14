

- SwiftUI
-  TableColumn 

Structure

# TableColumn

A column that displays a view for each row in a table.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
struct TableColumn where RowValue : Identifiable, Sort : SortComparator, Content : View, Label : View
```

## Overview

You create a column with a label, content view, and optional key path. The table calls the content view builder with the value for each row in the table. The column uses a key path to map to a property of each row value, which sortable tables use to reflect the current sort order.

The following example creates a sortable column for a table with `Person` rows, displaying each person’s given name:

```
TableColumn("Given name", value: \.givenName) { person in
    Text(person.givenName)
}
```

For the common case of `String` properties, you can use the convenience initializer that doesn’t require an explicit content closure and displays that string verbatim as a Text view. This means you can write the previous example as:

```
TableColumn("Given name", value: \.givenName)
```

## Topics

### Creating an unsortable column

init(_:value:)

Creates an unsortable column that displays a string property with a text label.

init(_:content:)

Creates an unsortable column with a text label

### Creating a sortable column

init(_:value:content:)

Creates a sortable column for Boolean values with a text label.

init(_:value:comparator:)

Creates a sortable column that displays a string property and has a text label.

init(_:value:comparator:content:)

Creates a sortable column with a text label.

init(_:sortUsing:content:)

Creates a sortable column with text label.

### Setting the column width

func width(CGFloat?) -> TableColumn&lt;RowValue, Sort, Content, Label>

Creates a fixed width table column that isn’t user resizable.

func width(min: CGFloat?, ideal: CGFloat?, max: CGFloat?) -> TableColumn&lt;RowValue, Sort, Content, Label>

Creates a resizable table column with the provided constraints.

func width() -> TableColumn&lt;RowValue, Sort, Content, Label>

Sets the column’s width.

Deprecated

## Relationships

### Conforms To

- TableColumnContent

## See Also

### Creating columns

protocol TableColumnContent

A type used to represent columns within a table.

struct TableColumnAlignment

Describes the alignment of the content of a table column.

struct TableColumnBuilder

A result builder that creates table column content from closures.

struct TableColumnForEach

A structure that computes columns on demand from an underlying collection of identified data.

