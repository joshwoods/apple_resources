

- UIKit
- UIScrollView
-  scrollRectToVisible(\_:animated:) 

Instance Method

# scrollRectToVisible(\_:animated:)

Scrolls a specific area of the content so that it’s visible in the scroll view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scrollRectToVisible(
    _ rect: CGRect,
    animated: Bool
)
```

## Parameters 

`rect`  

A rectangle defining an area of the content view. The rectangle should be in the coordinate space of the scroll view.

`animated`  

true if the scrolling should be animated, false if it should be immediate.

## Discussion

This method scrolls the content view so that the area defined by `rect` is just visible inside the scroll view. If the area is already visible, the method does nothing.

