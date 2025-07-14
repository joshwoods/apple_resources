

- FinanceKitUI
- AddOrderToWalletButton
-  windowToolbarFullScreenVisibility(\_:) 

Instance Method

# windowToolbarFullScreenVisibility(\_:)

Configures the visibility of the window toolbar when the window enters full screen mode.

FinanceKitUISwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func windowToolbarFullScreenVisibility(_ visibility: WindowToolbarFullScreenVisibility) -> some View
```

## Parameters 

`visibility`  

The visibility to use for the window toolbar in full screen mode.

## Discussion

By default, the window toolbar will show at the top of the display, above the window’s contents.

You can use this modifier to override the default behavior.

For example, you can specify that the window toolbar should be hidden by default, and only show once the mouse moves into the area occupied by the menu bar:

```
struct RootView: View {
    var body: some View {
        ContentView()
            .toolbar {
                ...
            }
            .windowToolbarFullScreenVisibility(.onHover)
    }
}
```

