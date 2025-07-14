

- UIKit
- UIScrollViewDelegate
-  viewForZooming(in:) 

Instance Method

# viewForZooming(in:)

Asks the delegate for the view to scale when zooming is about to occur in the scroll view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func viewForZooming(in scrollView: UIScrollView) -> UIView?
```

## Parameters 

`scrollView`  

The scroll-view object displaying the content view.

## Return Value

A UIView object that will be scaled as a result of the zooming gesture. Return `nil` if you don’t want zooming to occur.

## See Also

### Managing zooming

func scrollViewWillBeginZooming(UIScrollView, with: UIView?)

Tells the delegate that zooming of the content in the scroll view is about to commence.

func scrollViewDidEndZooming(UIScrollView, with: UIView?, atScale: CGFloat)

Tells the delegate when zooming of the content in the scroll view completed.

func scrollViewDidZoom(UIScrollView)

Tells the delegate that the scroll view’s zoom factor changed.

