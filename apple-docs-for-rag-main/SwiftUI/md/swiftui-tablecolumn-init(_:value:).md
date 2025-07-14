

- SwiftUI
- TableColumn
-  init(\_:value:) 

Initializer

# init(\_:value:)

Creates an unsortable column that displays a string property with a text label.

iOS 16.6+iPadOS 16.6+Mac Catalyst 16.6+macOS 13.5+visionOS 1.0+

``` source
nonisolated
init(
    _ text: Text,
    value: KeyPath
) where Content == Text
```

Available when `RowValue` conforms to `Identifiable`, `Sort` is `Never`, `Content` conforms to `View`, and `Label` is `Text`.

Show all declarations

## Parameters 

`text`  

The column’s label.

`value`  

The path to the property associated with the column. The table uses this to display the property as verbatim text in each row of the table.

## Discussion

This initializer creates a Text view for you, and treats the localized key similar to init(_:tableName:bundle:comment:). For more information about localizing strings, see Text.

## See Also

### Creating an unsortable column

init(_:content:)

Creates an unsortable column with a text label

