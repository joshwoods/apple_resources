

- UIKit
- UIScrollViewDelegate
-  scrollViewWillEndDragging(\_:withVelocity:targetContentOffset:) 

Instance Method

# scrollViewWillEndDragging(\_:withVelocity:targetContentOffset:)

Tells the delegate when the user finishes scrolling the content.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewWillEndDragging(
    _ scrollView: UIScrollView,
    withVelocity velocity: CGPoint,
    targetContentOffset: UnsafeMutablePointer
)
```

## Parameters 

`scrollView`  

The scroll-view object where the user ended the touch.

`velocity`  

The velocity of the scroll view (in points per millisecond) at the moment the touch was released.

`targetContentOffset`  

The expected offset when the scrolling action decelerates to a stop.

## Discussion

Your application can change the value of the `targetContentOffset` parameter to adjust where the scrollview finishes its scrolling animation.

## See Also

### Responding to scrolling and dragging

func scrollViewDidScroll(UIScrollView)

Tells the delegate when the user scrolls the content view within the scroll view.

func scrollViewWillBeginDragging(UIScrollView)

Tells the delegate when the scroll view is about to start scrolling the content.

func scrollViewDidEndDragging(UIScrollView, willDecelerate: Bool)

Tells the delegate when dragging ended in the scroll view.

func scrollViewShouldScrollToTop(UIScrollView) -> Bool

Asks the delegate if the scroll view should scroll to the top of the content.

func scrollViewDidScrollToTop(UIScrollView)

Tells the delegate that the scroll view scrolled to the top of the content.

func scrollViewWillBeginDecelerating(UIScrollView)

Tells the delegate that the scroll view is starting to decelerate the scrolling movement.

func scrollViewDidEndDecelerating(UIScrollView)

Tells the delegate that the scroll view ended decelerating the scrolling movement.

