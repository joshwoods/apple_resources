

- SwiftUI
-  ContextMenu Deprecated

Structure

# ContextMenu

A container for views that you present as menu items in a context menu.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–7.0Deprecated

``` source
struct ContextMenu where MenuItems : View
```

Deprecated

Use contextMenu(menuItems:) instead.

## Overview

A context menu view allows you to present a situationally specific menu that enables taking actions relevant to the current task.

You can create a context menu by first defining a `ContextMenu` container with the controls that represent the actions people can take, and then using the contextMenu(_:) view modifier to apply the menu to a view.

The example below creates and applies a two item context menu container to a Text view. The Boolean value `shouldShowMenu`, which defaults to true, controls the availability of context menu:

```
private let menuItems = ContextMenu {
    Button {
        // Add this item to a list of favorites.
    } label: {
        Label("Add to Favorites", systemImage: "heart")
    }
    Button {
        // Open Maps and center it on this item.
    } label: {
        Label("Show in Maps", systemImage: "mappin")
    }
}

private struct ContextMenuMenuItems: View {
    @State private var shouldShowMenu = true

    var body: some View {
        Text("Turtle Rock")
            .contextMenu(shouldShowMenu ? menuItems : nil)
    }
}
```

## Topics

### Creating a context menu

init(menuItems: () -> MenuItems)

Creates a context menu.

## See Also

### Deprecated types

struct MenuButton

A button that displays a menu containing a list of choices when pressed.

Deprecated

typealias PullDownButtonDeprecated

