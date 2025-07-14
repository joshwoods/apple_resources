

- UIKit
- UIScrollView
- UIScrollView.ContentInsetAdjustmentBehavior
-  UIScrollView.ContentInsetAdjustmentBehavior.automatic 

Case

# UIScrollView.ContentInsetAdjustmentBehavior.automatic

Automatically adjust the scroll view insets.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
case automatic
```

## Discussion

Content is always adjusted vertically when the scroll view is the content view of a view controller that is currently displayed by a navigation or tab bar controller. If the scroll view is horizontally scrollable, the horizontal content offset is also adjusted when there are nonzero safe area insets.

