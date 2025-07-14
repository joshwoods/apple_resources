

- UIKit
- UIScrollViewDelegate
-  scrollViewDidEndZooming(\_:with:atScale:) 

Instance Method

# scrollViewDidEndZooming(\_:with:atScale:)

Tells the delegate when zooming of the content in the scroll view completed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func scrollViewDidEndZooming(
    _ scrollView: UIScrollView,
    with view: UIView?,
    atScale scale: CGFloat
)
```

## Parameters 

`scrollView`  

The scroll-view object displaying the content view.

`view`  

The view object representing that part of the content view that needs to be scaled.

`scale`  

The scale factor to use for scaling; this value must be between the limits established by the `UIScrollView` properties maximumZoomScale and minimumZoomScale.

## Discussion

The scroll view also calls this method after any “bounce” animations. It also calls this method after animated changes to the zoom level and after a zoom-related gesture ends (regardless of whether the gesture resulted in a change to the zoom level).

## See Also

### Managing zooming

func viewForZooming(in: UIScrollView) -> UIView?

Asks the delegate for the view to scale when zooming is about to occur in the scroll view.

func scrollViewWillBeginZooming(UIScrollView, with: UIView?)

Tells the delegate that zooming of the content in the scroll view is about to commence.

func scrollViewDidZoom(UIScrollView)

Tells the delegate that the scroll view’s zoom factor changed.

