

- SwiftUI
- UIHostingController
-  preferredContentSizeDidChange(forChildContentContainer:) 

Instance Method

# preferredContentSizeDidChange(forChildContentContainer:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
override dynamic func preferredContentSizeDidChange(forChildContentContainer container: any UIContentContainer)
```

## See Also

### Managing the size

var sizingOptions: UIHostingControllerSizingOptions

The options for how the hosting controller tracks changes to the size of its SwiftUI content.

func sizeThatFits(in: CGSize) -> CGSize

Calculates and returns the most appropriate size for the current view.

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

