

- SwiftUI
- TableColumn
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates an unsortable column with a text label

iOS 16.6+iPadOS 16.6+Mac Catalyst 16.6+macOS 13.5+visionOS 1.0+

``` source
nonisolated
init(
    _ text: Text,
    @ViewBuilder content: @escaping (RowValue) -> Content
)
```

Available when `RowValue` conforms to `Identifiable`, `Sort` is `Never`, `Content` conforms to `View`, and `Label` is `Text`.

Show all declarations

## Parameters 

`text`  

The column’s label.

`content`  

The view content to display for each row in a table.

## Discussion

This initializer creates a Text view for you, and treats the title similar to init(_:). For information about localizing strings, see Text.

## See Also

### Creating an unsortable column

init(_:value:)

Creates an unsortable column that displays a string property with a text label.

