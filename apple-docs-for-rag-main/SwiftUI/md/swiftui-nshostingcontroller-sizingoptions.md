

- SwiftUI
- NSHostingController
-  sizingOptions 

Instance Property

# sizingOptions

The options for how the hosting controller’s view creates and updates constraints based on the size of its SwiftUI content.

macOS 13.0+

``` source
@MainActor @preconcurrency
var sizingOptions: NSHostingSizingOptions { get set }
```

## Discussion

NSHostingController can create minimum, maximum, and ideal (content size) constraints that are derived from its SwiftUI view content. These constraints are only created when Auto Layout constraints are otherwise being used in the containing window.

If the NSHostingController is set as the `contentViewController` of an `NSWindow`, it will also update the window’s `contentMinSize` and `contentMaxSize` based on the minimum and maximum size of its SwiftUI content.

`sizingOptions` defaults to `.standardBounds` (which includes `minSize`, `intrinsicContentSize`, and `maxSize`), but can be set to an explicit value to control this behavior. For instance, setting a value of `.minSize` will only create the constraints necessary to maintain the minimum size of the SwiftUI content, or setting a value of `[]` will create no constraints at all.

If a use case can make assumptions about the size of the `NSHostingController` relative to its displayed content, such as the always being displayed in a fixed frame, setting this to a value with fewer options can improve performance as it reduces the amount of layout measurements that need to be performed. If an `NSHostingController` has a `frame` that is smaller or larger than that required to display its SwiftUI content, the content will be centered within that frame.

## See Also

### Configuring the controller

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var preferredContentSize: NSSize

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

var sceneBridgingOptions: NSHostingSceneBridgingOptions

The options for which aspects of the window will be managed by this controller’s hosting view.

