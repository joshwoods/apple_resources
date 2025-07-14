

- SwiftUI
- View
-  statusBar(hidden:) Deprecated

Instance Method

# statusBar(hidden:)

Sets the visibility of the status bar.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
nonisolated
func statusBar(hidden: Bool) -> some View
```

Deprecated

Use statusBarHidden(_:) instead.

## Discussion

Use this method to show or hide the status bar.

## See Also

### Auxiliary view modifiers

func navigationBarTitle(_:)

Sets the title in the navigation bar for this view.

Deprecated

func navigationBarTitle(_:displayMode:)

Sets the title and display mode in the navigation bar for this view.

Deprecated

func navigationBarItems&lt;L>(leading: L) -> some View

Sets the navigation bar items for this view.

Deprecated

func navigationBarItems&lt;L, T>(leading: L, trailing: T) -> some View

Sets the navigation bar items for this view.

Deprecated

func navigationBarItems&lt;T>(trailing: T) -> some View

Configures the navigation bar items for this view.

Deprecated

func navigationBarHidden(Bool) -> some View

Hides the navigation bar for this view.

Deprecated

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

Deprecated

