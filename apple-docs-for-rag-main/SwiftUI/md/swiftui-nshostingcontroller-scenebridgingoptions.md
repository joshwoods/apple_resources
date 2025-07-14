

- SwiftUI
- NSHostingController
-  sceneBridgingOptions 

Instance Property

# sceneBridgingOptions

The options for which aspects of the window will be managed by this controller’s hosting view.

macOS 14.0+

``` source
@MainActor @preconcurrency
var sceneBridgingOptions: NSHostingSceneBridgingOptions { get set }
```

## Discussion

`NSHostingController` will populate certain aspects of its associated window, depending on which options are specified.

For example, a hosting controller can manage its window’s toolbar by including the `.toolbars` option:

```
struct RootView: View {
    var body: some View {
        ContentView()
            .toolbar {
                MyToolbarContent()
            }
    }
}

let controller = NSHostingController(rootView: RootView())
controller.sceneBridgingOptions = [.toolbars]
```

When this hosting controller is set as the `contentViewController` for a window, the default value for this property will be `.all`, which includes the options for `.toolbars` and `.title`. Otherwise, the default value is `[]`.

## See Also

### Configuring the controller

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var preferredContentSize: NSSize

var sizingOptions: NSHostingSizingOptions

The options for how the hosting controller’s view creates and updates constraints based on the size of its SwiftUI content.

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

