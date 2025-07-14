

- UIKit
- UIScrollViewDelegate
-  scrollViewWillBeginZooming(\_:with:) 

Instance Method

# scrollViewWillBeginZooming(\_:with:)

Tells the delegate that zooming of the content in the scroll view is about to commence.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewWillBeginZooming(
    _ scrollView: UIScrollView,
    with view: UIView?
)
```

## Parameters 

`scrollView`  

The scroll-view object displaying the content view.

`view`  

The view object whose content is about to be zoomed.

## Discussion

This method is called at the beginning of zoom gestures and in cases where a change in zoom level is to be animated. You can use this method to store state information or perform any additional actions prior to zooming the view’s content.

## See Also

### Managing zooming

func viewForZooming(in: UIScrollView) -> UIView?

Asks the delegate for the view to scale when zooming is about to occur in the scroll view.

func scrollViewDidEndZooming(UIScrollView, with: UIView?, atScale: CGFloat)

Tells the delegate when zooming of the content in the scroll view completed.

func scrollViewDidZoom(UIScrollView)

Tells the delegate that the scroll view’s zoom factor changed.

