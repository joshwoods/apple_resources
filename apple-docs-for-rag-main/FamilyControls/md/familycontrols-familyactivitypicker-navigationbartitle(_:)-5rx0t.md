

- FamilyControls
- FamilyActivityPicker
-  navigationBarTitle(\_:) 

Instance Method

# navigationBarTitle(\_:)

Sets the title of this view’s navigation bar with a string.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func navigationBarTitle(_ title: S) -> some View where S : StringProtocol
```

## Parameters 

`title`  

A title for this view to display in the navigation bar.

## Discussion

Use `navigationBarTitle(_:)` to set the title of the navigation bar using a `String`. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

In the example below, text for the navigation bar title is provided using a string:

```
struct FlavorView: View {
    let items = ["Chocolate", "Vanilla", "Strawberry", "Mint Chip",
                 "Pistachio"]
    let text = "Today's Flavors"
    var body: some View {
        NavigationView {
            List(items, id: \.self) {
                Text($0)
            }
            .navigationBarTitle(text)
        }
    }
}
```

## See Also

### Deprecated Auxiliary View Modifiers

func navigationBarTitle(LocalizedStringKey) -> some View

Sets the title of this view’s navigation bar with a localized string.

func navigationBarTitle(Text) -> some View

Sets the title in the navigation bar for this view.

func navigationBarTitle(Text, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarTitle&lt;S>(S, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarTitle(LocalizedStringKey, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarItems&lt;L>(leading: L) -> some View

func navigationBarItems&lt;L, T>(leading: L, trailing: T) -> some View

func navigationBarItems&lt;T>(trailing: T) -> some View

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

