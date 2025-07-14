

- SwiftUI
- NSHostingController
-  preferredContentSize 

Instance Property

# preferredContentSize

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic var preferredContentSize: NSSize { get set }
```

## See Also

### Configuring the controller

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var sizingOptions: NSHostingSizingOptions

The options for how the hosting controller’s view creates and updates constraints based on the size of its SwiftUI content.

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

var sceneBridgingOptions: NSHostingSceneBridgingOptions

The options for which aspects of the window will be managed by this controller’s hosting view.

