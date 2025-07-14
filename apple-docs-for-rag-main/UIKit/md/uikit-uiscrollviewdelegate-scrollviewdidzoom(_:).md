

- UIKit
- UIScrollViewDelegate
-  scrollViewDidZoom(\_:) 

Instance Method

# scrollViewDidZoom(\_:)

Tells the delegate that the scroll view’s zoom factor changed.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewDidZoom(_ scrollView: UIScrollView)
```

## Parameters 

`scrollView`  

The scroll-view object whose zoom factor changed.

## See Also

### Managing zooming

func viewForZooming(in: UIScrollView) -> UIView?

Asks the delegate for the view to scale when zooming is about to occur in the scroll view.

func scrollViewWillBeginZooming(UIScrollView, with: UIView?)

Tells the delegate that zooming of the content in the scroll view is about to commence.

func scrollViewDidEndZooming(UIScrollView, with: UIView?, atScale: CGFloat)

Tells the delegate when zooming of the content in the scroll view completed.

