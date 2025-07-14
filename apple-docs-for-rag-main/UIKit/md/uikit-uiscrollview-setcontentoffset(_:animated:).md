

- UIKit
- UIScrollView
-  setContentOffset(\_:animated:) 

Instance Method

# setContentOffset(\_:animated:)

Sets the offset from the content view’s origin that corresponds to the scroll view’s origin.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setContentOffset(
    _ contentOffset: CGPoint,
    animated: Bool
)
```

## Parameters 

`contentOffset`  

A point (expressed in points) that’s offset from the content view’s origin.

`animated`  

true to animate the transition at a constant velocity to the new offset, false to make the transition immediate.

## See Also

### Managing the content size and offset

var contentSize: CGSize

The size of the content view.

var contentOffset: CGPoint

The point at which the origin of the content view is offset from the origin of the scroll view.

