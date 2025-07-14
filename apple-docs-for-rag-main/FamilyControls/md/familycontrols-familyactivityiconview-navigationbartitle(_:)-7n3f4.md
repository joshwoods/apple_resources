

- FamilyControls
- FamilyActivityIconView
-  navigationBarTitle(\_:) 

Instance Method

# navigationBarTitle(\_:)

Sets the title in the navigation bar for this view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func navigationBarTitle(_ title: Text) -> some View
```

## Parameters 

`title`  

A description of this view to display in the navigation bar.

## Discussion

Use `navigationBarTitle(_:)` to set the title of the navigation bar. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

The example below shows setting the title of the navigation bar using a `Text` view:

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

