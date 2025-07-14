

- SwiftUI
- TabContent
-  contextMenu(menuItems:) 

Instance Method

# contextMenu(menuItems:)

Adds a context menu to a tab.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
func contextMenu(@ViewBuilder menuItems: () -> M) -> some TabContent where M : View
```

## Parameters 

`menuItems`  

A closure that produces the menu’s contents. You can deactivate the context menu by returning nothing from the closure.

## Return Value

A row that can display a context menu.

## Discussion

Use this modifier to add a context menu to a tab’s sidebar representation. Compose the menu by returning controls like Button, Toggle and Picker from the `menuItems` closure. You can also use Menu to define submenus, or Section to group items.

The following example adds the ability to pin the tab or share the tab’s books with a friend.

```
Tab("Currently Reading", systemImage: "book") {
    CurrentBooksList()
}
.contextMenu {
    Button {
        // Pin this tab.
    } label: {
        Label("Pin", systemImage: "pin")
    }
    Button {
        // Open a share sheet to share
    } label: {
        Label("Share", systemImage: "square.and.arrow.up")
    }
}
```

