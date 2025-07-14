

- UIKit
- UIScrollView
- UIScrollView.ContentInsetAdjustmentBehavior
-  UIScrollView.ContentInsetAdjustmentBehavior.scrollableAxes 

Case

# UIScrollView.ContentInsetAdjustmentBehavior.scrollableAxes

Adjust the insets only in the scrollable directions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
case scrollableAxes
```

## Discussion

The top and bottom insets include the safe area inset values when the vertical content size is greater than the height of the scroll view itself. The top and bottom insets are also adjusted when the alwaysBounceVertical property is true. Similarly, the left and right insets include the safe area insets when the horizontal content size is greater than the width of the scroll view.

