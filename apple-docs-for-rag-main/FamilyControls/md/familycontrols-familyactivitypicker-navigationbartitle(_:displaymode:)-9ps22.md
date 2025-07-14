

- FamilyControls
- FamilyActivityPicker
-  navigationBarTitle(\_:displayMode:) 

Instance Method

# navigationBarTitle(\_:displayMode:)

Sets the title and display mode in the navigation bar for this view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedvisionOS 1.0+

``` source
nonisolated
func navigationBarTitle(
    _ titleKey: LocalizedStringKey,
    displayMode: NavigationBarItem.TitleDisplayMode
) -> some View
```

## Parameters 

`titleKey`  

A key to a localized description of this view to display in the navigation bar.

`displayMode`  

The style to use for displaying the navigation bar title.

## Discussion

Use `navigationBarTitle(_:displayMode:)` to set the title of the navigation bar for this view and specify a display mode for the title from one of the `NavigationBarItem/TitleDisplayMode` styles. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

In the example below, text for the navigation bar title is provided using a string. The navigation bar title’s `NavigationBarItem/TitleDisplayMode` is set to `.inline` which places the navigation bar title in the bounds of the navigation bar.

```
struct FlavorView: View {
    let items = ["Chocolate", "Vanilla", "Strawberry", "Mint Chip",
                 "Pistachio"]
    var body: some View {
        NavigationView {
            List(items, id: \.self) {
                Text($0)
            }
            .navigationBarTitle("Today's Flavors", displayMode: .inline)
        }
    }
}
```

If the `titleKey` can’t be found, the title uses the text of the key name instead.

## See Also

### Deprecated Auxiliary View Modifiers

func navigationBarTitle&lt;S>(S) -> some View

Sets the title of this view’s navigation bar with a string.

func navigationBarTitle(LocalizedStringKey) -> some View

Sets the title of this view’s navigation bar with a localized string.

func navigationBarTitle(Text) -> some View

Sets the title in the navigation bar for this view.

func navigationBarTitle(Text, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarTitle&lt;S>(S, displayMode: NavigationBarItem.TitleDisplayMode) -> some View

Sets the title and display mode in the navigation bar for this view.

func navigationBarItems&lt;L>(leading: L) -> some View

func navigationBarItems&lt;L, T>(leading: L, trailing: T) -> some View

func navigationBarItems&lt;T>(trailing: T) -> some View

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

