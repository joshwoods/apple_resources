

- FinanceKitUI
- AddOrderToWalletButton
-  toolbar(\_:for:) 

Instance Method

# toolbar(\_:for:)

Specifies the visibility of a bar managed by SwiftUI.

FinanceKitUISwiftUIiOS 16.0–18.4DeprecatediPadOS 16.0–18.4DeprecatedMac Catalyst 16.0–18.4DeprecatedmacOS 13.0–15.4DeprecatedtvOS 16.0+watchOS 9.0+

``` source
nonisolated
func toolbar(
    _ visibility: Visibility,
    for bars: ToolbarPlacement...
) -> some View
```

## Parameters 

`visibility`  

The preferred visibility of the bar.

`bars`  

The bars to update the visibility of or `ToolbarPlacement/automatic` if empty.

## Discussion

The preferred visibility flows up to the nearest container that renders a bar. This could be a `NavigationView` or `TabView` in iOS, or the root view of a `WindowGroup` in macOS.

This examples shows a view that hides the navigation bar on iOS, or the window toolbar items on macOS.

```
NavigationView {
    ContentView()
        .toolbar(.hidden)
}
```

To hide the entire titlebar on macOS, use this modifier with `ToolbarPlacement/windowToolbar` placement.

```
NavigationView {
    ContentView()
        .toolbar(.hidden, for: .windowToolbar)
}
```

You can provide multiple `ToolbarPlacement` instances to hide multiple bars at once.

```
TabView {
    NavigationView {
        ContentView()
            .toolbar(
                .hidden, for: .navigationBar, .tabBar)
    }
}
```

Note

In macOS, if you provide `ToolbarCommands` to the scene of your app, this modifier disables the toolbar visibility command while the value of the modifier is not `ToolbarPlacement/automatic`.

Depending on the specified bars, the requested visibility may not be able to be fulfilled.

