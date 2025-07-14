

- SwiftUI
- NSHostingController
-  safeAreaRegions 

Instance Property

# safeAreaRegions

The safe area regions that this view controller adds to its view.

macOS 13.3+

``` source
@MainActor @preconcurrency
var safeAreaRegions: SafeAreaRegions { get set }
```

## Discussion

The default value is `SafeAreaRegions.all`.

## See Also

### Configuring the controller

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var preferredContentSize: NSSize

var sizingOptions: NSHostingSizingOptions

The options for how the hosting controller’s view creates and updates constraints based on the size of its SwiftUI content.

var sceneBridgingOptions: NSHostingSceneBridgingOptions

The options for which aspects of the window will be managed by this controller’s hosting view.

