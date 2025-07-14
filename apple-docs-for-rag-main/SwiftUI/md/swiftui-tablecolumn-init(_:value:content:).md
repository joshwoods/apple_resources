

- SwiftUI
- TableColumn
-  init(\_:value:content:) 

Initializer

# init(\_:value:content:)

Creates a sortable column for Boolean values with a text label.

iOS 16.6+iPadOS 16.6+Mac Catalyst 16.6+macOS 13.5+visionOS 1.0+

``` source
init(
    _ text: Text,
    value: KeyPath,
    @ViewBuilder content: @escaping (RowValue) -> Content
)
```

Available when `RowValue` inherits `NSObject`, `RowValue` conforms to `Identifiable`, `Sort` is `SortDescriptor`, `Content` conforms to `View`, and `Label` is `Text`.

Show all declarations

## Parameters 

`text`  

The column’s label.

`value`  

The path to the property associated with the column, which will be used to update and reflect the sorting state in a table.

`content`  

The view content to display for each row in a table.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Creating a sortable column

init(_:value:comparator:)

Creates a sortable column that displays a string property and has a text label.

init(_:value:comparator:content:)

Creates a sortable column with a text label.

init(_:sortUsing:content:)

Creates a sortable column with text label.

