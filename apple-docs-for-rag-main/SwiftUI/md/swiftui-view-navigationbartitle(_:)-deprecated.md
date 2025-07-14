

- SwiftUI
- View
-  navigationBarTitle(\_:) Deprecated

Instance Method

# navigationBarTitle(\_:)

Sets the title in the navigation bar for this view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func navigationBarTitle(_ title: Text) -> some View
```

Deprecated

Use navigationTitle(_:) instead.

Show all declarations

## Parameters 

`title`  

A description of this view to display in the navigation bar.

## Discussion

Use `navigationBarTitle(_:)` to set the title of the navigation bar. This modifier only takes effect when this view is inside of and visible within a NavigationView.

The example below shows setting the title of the navigation bar using a Text view:

```
struct FlavorView: View {
    let items = ["Chocolate", "Vanilla", "Strawberry", "Mint Chip",
                 "Pistachio"]
    var body: some View {
        NavigationView {
            List(items, id: \.self) {
                Text($0)
            }
            .navigationBarTitle(Text("Today's Flavors"))
        }
    }
}
```

## See Also

### Auxiliary view modifiers

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

func statusBar(hidden: Bool) -> some View

Sets the visibility of the status bar.

Deprecated

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

Deprecated

