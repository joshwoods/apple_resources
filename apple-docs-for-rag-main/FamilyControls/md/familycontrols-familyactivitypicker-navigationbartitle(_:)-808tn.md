

- FamilyControls
- FamilyActivityPicker
-  navigationBarTitle(\_:) 

Instance Method

# navigationBarTitle(\_:)

Sets the title of this view’s navigation bar with a localized string.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func navigationBarTitle(_ titleKey: LocalizedStringKey) -> some View
```

## Parameters 

`titleKey`  

A key to a localized description of this view to display in the navigation bar.

## Discussion

Use `navigationBarTitle(_:)` to set the title of the navigation bar using a `LocalizedStringKey` that will be used to search for a matching localized string in the application’s localizable strings assets.

This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

In the example below, a string constant is used to access a `LocalizedStringKey` that will be resolved at run time to provide a title for the navigation bar. If the localization key cannot be resolved, the text of the key name will be used as the title text.

```
struct FlavorView: View {
    let items = ["Chocolate", "Vanilla", "Strawberry", "Mint Chip",
                 "Pistachio"]
    var body: some View {
        NavigationView {
            List(items, id: \.self) {
                Text($0)
            }
            .navigationBarTitle("Today's Flavors")
        }
    }
}
```

## See Also

### Deprecated Auxiliary View Modifiers

func navigationBarTitle&lt;S>(S) -> some View

Sets the title of this view’s navigation bar with a string.

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

