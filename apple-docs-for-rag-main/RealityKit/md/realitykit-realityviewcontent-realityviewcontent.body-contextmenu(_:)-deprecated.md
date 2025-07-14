

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  contextMenu(\_:) Deprecated

Instance Method

# contextMenu(\_:)

Adds a context menu to the view.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–7.0Deprecated

``` source
nonisolated
func contextMenu(_ contextMenu: ContextMenu?) -> some View where MenuItems : View
```

Deprecated

Use \`contextMenu(menuItems:)\` instead.

## Parameters 

`contextMenu`  

A context menu container for views that you present as menu items in a context menu.

## Return Value

A view that can show a context menu.

## Discussion

Use this method to attach a specified context menu to a view. You can make the context menu unavailable by conditionally passing `nil` as the value for the `contextMenu`.

The example below creates a `ContextMenu` that contains two items and passes them into the modifier. The Boolean value `shouldShowMenu`, which defaults to `true`, controls the context menu availability:

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

To customize the default preview, apply a `View/contentShape(_:_:eoFill:)` with a `ContentShapeKinds/contextMenuPreview` kind. For example, you can change the preview’s corner radius or use a nested view as the preview.

