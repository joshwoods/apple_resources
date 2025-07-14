

- SwiftUI
- TableRowContent
-  contextMenu(menuItems:preview:) 

Instance Method

# contextMenu(menuItems:preview:)

Adds a context menu with a preview to a table row.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func contextMenu(
    @ViewBuilder menuItems: () -> M,
    @ViewBuilder preview: () -> P
) -> ModifiedContent> where M : View, P : View
```

## Parameters 

`menuItems`  

A closure that produces the menu’s contents. You can deactivate the context menu by returning nothing from the closure.

`preview`  

A view that the system displays along with the menu.

## Return Value

A row that can display a context menu with a preview.

## Discussion

When you use this modifier to add a context menu to rows in a table, the system shows a preview beside the menu. Compose the menu by returning controls like Button, Toggle, and Picker from the `menuItems` closure. You can also use Menu to define submenus.

Define the preview by returning a view from the `preview` closure. The system sizes the preview to match the size of its content. For example, the following code adds a context menu with a preview to each row in a table that people can use to send an email to the person represented by that row:

```
Table(of: Person.self) {
    TableColumn("Given Name", value: \.givenName)
    TableColumn("Family Name", value: \.familyName)
} rows: {
    ForEach(people) { person in
        TableRow(person)
            .contextMenu {
                Button("Send Email...") { }
            } preview: {
                Image("envelope") // Loads the image from an asset catalog.
            }
    }
}
```

Note

This view modifier produces a context menu on macOS, but that platform doesn’t display the preview.

If you don’t need a preview, use contextMenu(menuItems:). If you want to display a context menu that’s based on the current selection, use contextMenu(forSelectionType:menu:primaryAction:). To add context menus to other kinds of views, see contextMenu(menuItems:).

## See Also

### Adding a context menu to a row

func contextMenu&lt;M>(menuItems: () -> M) -> ModifiedContent&lt;Self, _ContextMenuTableRowModifier&lt;M>>

Adds a context menu to a table row.

