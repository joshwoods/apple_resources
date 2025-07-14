

- SwiftUI
- UIHostingController
-  safeAreaRegions 

Instance Property

# safeAreaRegions

The safe area regions that this view controller adds to its view.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+tvOS 16.4+visionOS 1.0+

``` source
@MainActor @preconcurrency
var safeAreaRegions: SafeAreaRegions { get set }
```

Available when `Content` conforms to `View`.

## Discussion

An example of when this is appropriate to use is when hosting content that you know should never be affected by the safe area, such as a custom scrollable container. Disabling a safe area region omits it from the SwiftUI layout system altogether.

The default value is `SafeAreaRegions.all`.

## See Also

### Managing the size

var sizingOptions: UIHostingControllerSizingOptions

The options for how the hosting controller tracks changes to the size of its SwiftUI content.

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

