

- Assignables
- AssignableDocumentView
-  navigationBarTitle(\_:displayMode:) 

Instance Method

# navigationBarTitle(\_:displayMode:)

Sets the title and display mode in the navigation bar for this view.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
nonisolated
func navigationBarTitle(
    _ title: Text,
    displayMode: NavigationBarItem.TitleDisplayMode
) -> some View
```

## Parameters 

`title`  

A title for this view to display in the navigation bar.

`displayMode`  

The style to use for displaying the navigation bar title.

## Discussion

Use `navigationBarTitle(_:displayMode:)` to set the title of the navigation bar for this view and specify a display mode for the title from one of the `NavigationBarItem/TitleDisplayMode` styles. This modifier only takes effect when this view is inside of and visible within a `NavigationView`.

In the example below, text for the navigation bar title is provided using a `Text` view. The navigation bar title’s `NavigationBarItem/TitleDisplayMode` is set to `.inline` which places the navigation bar title in the bounds of the navigation bar.

```
struct FlavorView: View {
   let items = ["Chocolate", "Vanilla", "Strawberry", "Mint Chip",
                "Pistachio"]
   var body: some View {
        NavigationView {
            List(items, id: \.self) {
                Text($0)
            }
            .navigationBarTitle(Text("Today's Flavors", displayMode: .inline)
        }
    }
}
```

