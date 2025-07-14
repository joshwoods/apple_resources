

- SwiftUI
- TableColumn
-  init(\_:sortUsing:content:) 

Initializer

# init(\_:sortUsing:content:)

Creates a sortable column with text label.

iOS 16.6+iPadOS 16.6+Mac Catalyst 16.6+macOS 13.5+visionOS 1.0+

``` source
nonisolated
init(
    _ text: Text,
    sortUsing comparator: Sort,
    @ViewBuilder content: @escaping (RowValue) -> Content
)
```

Available when `RowValue` conforms to `Identifiable`, `RowValue` is `Sort.Compared`, `Sort` conforms to `SortComparator`, `Content` conforms to `View`, and `Label` is `Text`.

Show all declarations

## Parameters 

`text`  

The column’s label.

`comparator`  

The prototype sort comparator to use when representing this column. When a person taps or clicks the column header, the containing table’s `sortOrder` incorporates this value, potentially with a flipped order.

`content`  

The view content to display for each row in a table.

## Discussion

This initializer creates a Text view for you, and treats the title similar to init(_:). For more information about localizing strings, see Text.

## See Also

### Creating a sortable column

init(_:value:content:)

Creates a sortable column for Boolean values with a text label.

init(_:value:comparator:)

Creates a sortable column that displays a string property and has a text label.

init(_:value:comparator:content:)

Creates a sortable column with a text label.

