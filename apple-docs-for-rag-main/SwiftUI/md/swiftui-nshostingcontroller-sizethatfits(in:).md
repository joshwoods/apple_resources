

- SwiftUI
- NSHostingController
-  sizeThatFits(in:) 

Instance Method

# sizeThatFits(in:)

Calculates and returns the most appropriate size for the current view.

macOS 10.15+

``` source
@MainActor @preconcurrency
func sizeThatFits(in size: CGSize) -> CGSize
```

## Parameters 

`size`  

The proposed new size for the view.

## Return Value

The size that offers the best fit for the root view and its contents.

## See Also

### Configuring the controller

var preferredContentSize: NSSize

var sizingOptions: NSHostingSizingOptions

The options for how the hosting controller’s view creates and updates constraints based on the size of its SwiftUI content.

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

var sceneBridgingOptions: NSHostingSceneBridgingOptions

The options for which aspects of the window will be managed by this controller’s hosting view.

