

- SwiftUI
- TableColumn
-  init(\_:value:comparator:) 

Initializer

# init(\_:value:comparator:)

Creates a sortable column that displays a string property and has a text label.

iOS 16.6+iPadOS 16.6+Mac Catalyst 16.6+macOS 13.5+visionOS 1.0+

``` source
init(
    _ text: Text,
    value: KeyPath,
    comparator: String.StandardComparator = .localizedStandard
) where Content == Text
```

Available when `RowValue` conforms to `Identifiable`, `Sort` is `KeyPathComparator`, `Content` conforms to `View`, and `Label` is `Text`.

Show all declarations

## Parameters 

`text`  

The column’s label.

`value`  

The path to the property associated with the column, to display verbatim as text in each row of a table, and the key path used to create a sort comparator when sorting the column.

`comparator`  

The `SortComparator` used to order the string values.

## Discussion

This initializer creates a Text view for you, and treats the title similar to init(_:). For more information about localizing strings, see Text.

## See Also

### Creating a sortable column

init(_:value:content:)

Creates a sortable column for Boolean values with a text label.

init(_:value:comparator:content:)

Creates a sortable column with a text label.

init(_:sortUsing:content:)

Creates a sortable column with text label.

