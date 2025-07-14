

- SwiftUI
- TableRowContent
-  contextMenu(menuItems:) 

Instance Method

# contextMenu(menuItems:)

Adds a context menu to a table row.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func contextMenu(@ViewBuilder menuItems: () -> M) -> ModifiedContent> where M : View
```

## Parameters 

`menuItems`  

A closure that produces the menu’s contents. You can deactivate the context menu by returning nothing from the closure.

## Return Value

A row that can display a context menu.

## Discussion

Use this modifier to add a context menu to a table row. Compose the menu by returning controls like Button, Toggle, and Picker from the `menuItems` closure. You can also use Menu to define submenus, or Section to group items.

The following example adds a context menu to each row in a table that people can use to send an email to the person represented by that row:

```
Table(of: Person.self) {
    TableColumn("Given Name", value: \.givenName)
    TableColumn("Family Name", value: \.familyName)
} rows: {
    ForEach(people) { person in
        TableRow(person)
            .contextMenu {
                Button("Send Email...") { }
            }
    }
}
```

If you want to display a preview beside the context menu, use contextMenu(menuItems:preview:). If you want to display a context menu that’s based on the current selection, use contextMenu(forSelectionType:menu:primaryAction:). To add context menus to other kinds of views, use contextMenu(menuItems:).

## See Also

### Adding a context menu to a row

func contextMenu&lt;M, P>(menuItems: () -> M, preview: () -> P) -> ModifiedContent&lt;Self, _ContextMenuPreviewTableRowModifier&lt;M, P>>

Adds a context menu with a preview to a table row.

