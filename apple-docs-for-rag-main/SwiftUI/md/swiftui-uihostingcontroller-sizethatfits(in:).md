

- SwiftUI
- UIHostingController
-  sizeThatFits(in:) 

Instance Method

# sizeThatFits(in:)

Calculates and returns the most appropriate size for the current view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

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

### Managing the size

var sizingOptions: UIHostingControllerSizingOptions

The options for how the hosting controller tracks changes to the size of its SwiftUI content.

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

var safeAreaRegions: SafeAreaRegions

The safe area regions that this view controller adds to its view.

