

- SwiftUI
- UIHostingController
-  sizingOptions 

Instance Property

# sizingOptions

The options for how the hosting controller tracks changes to the size of its SwiftUI content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
var sizingOptions: UIHostingControllerSizingOptions { get set }
```

## Discussion

The default value is the empty set.

## See Also

### Managing the size

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

