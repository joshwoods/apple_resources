

- SwiftUI
- View
-  navigationBarItems(leading:trailing:) Deprecated

Instance Method

# navigationBarItems(leading:trailing:)

Sets the navigation bar items for this view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
nonisolated
func navigationBarItems(
    leading: L,
    trailing: T
) -> some View where L : View, T : View
```

Deprecated

Use toolbar(content:) with navigationBarLeading or navigationBarTrailing placement.

## Parameters 

`leading`  

A view that appears on the leading edge of the title.

`trailing`  

A view that appears on the trailing edge of the title.

## Discussion

Use `navigationBarItems(leading:trailing:)` to add navigation bar items to the leading and trailing edges of the navigation bar for this view.

This modifier only takes effect when this view is inside of and visible within a NavigationView.

On iOS 14 and later, the leading item supplements a visible back button, instead of replacing it, by default. To hide the back button, use navigationBarBackButtonHidden(_:).

The example below adds buttons to the leading and trailing edges of the button area of the navigation view:

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
            .navigationBarItems(leading:
                HStack {
                    Button("Hours") {
                        print("Hours tapped!")
                    }
                }, trailing:
                HStack {
                    Button("Favorites") {
                        print("Favorites tapped!")
                    }

                    Button("Specials") {
                        print("Specials tapped!")
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

