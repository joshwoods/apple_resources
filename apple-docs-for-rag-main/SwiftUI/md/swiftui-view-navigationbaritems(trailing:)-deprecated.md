

- SwiftUI
- View
-  navigationBarItems(trailing:) Deprecated

Instance Method

# navigationBarItems(trailing:)

Configures the navigation bar items for this view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
nonisolated
func navigationBarItems(trailing: T) -> some View where T : View
```

Deprecated

Use toolbar(content:) with navigationBarTrailing placement.

## Parameters 

`trailing`  

A view shown on the trailing edge of the title.

## Discussion

Use `navigationBarItems(trailing:)` to add navigation bar items to the trailing edge of the navigation bar for this view. This modifier only takes effect when this view is inside of and visible within a NavigationView.

The example below adds buttons to the trailing edge of the button area of the navigation view:

```
struct FlavorView: View {
    var body: some View {
        NavigationView {
            List {
                Text("Chocolate")
                Text("Vanilla")
                Text("Strawberry")
            }
            .navigationBarTitle(Text("Today‘s Flavors"))
            .navigationBarItems(trailing:
                HStack {
                    Button("Hours") {
                        print("Hours tapped!")
                    }

                    Button("Help") {
                        print("Help tapped!")
                    }
                }
            )
        }
    }
}
```

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

func navigationBarHidden(Bool) -> some View

Hides the navigation bar for this view.

Deprecated

func statusBar(hidden: Bool) -> some View

Sets the visibility of the status bar.

Deprecated

func contextMenu&lt;MenuItems>(ContextMenu&lt;MenuItems>?) -> some View

Adds a context menu to the view.

Deprecated

