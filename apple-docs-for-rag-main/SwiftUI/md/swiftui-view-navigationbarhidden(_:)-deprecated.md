

- SwiftUI
- View
-  navigationBarHidden(\_:) Deprecated

Instance Method

# navigationBarHidden(\_:)

Hides the navigation bar for this view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func navigationBarHidden(_ hidden: Bool) -> some View
```

Deprecated

Use toolbar(_:for:) with the Visibility.hidden visibility and the navigationBar placement instead.

## Parameters 

`hidden`  

A Boolean value that indicates whether to hide the navigation bar.

## Discussion

Use this method to hide the navigation bar. This modifier only takes effect when the modified view is inside of and visible within a NavigationView.

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

func statusBar(hidden: Bool) -> some View

Sets the visibility of the status bar.

Deprecated

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

Deprecated

