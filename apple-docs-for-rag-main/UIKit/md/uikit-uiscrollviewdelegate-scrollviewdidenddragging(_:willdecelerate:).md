

- UIKit
- UIScrollViewDelegate
-  scrollViewDidEndDragging(\_:willDecelerate:) 

Instance Method

# scrollViewDidEndDragging(\_:willDecelerate:)

Tells the delegate when dragging ended in the scroll view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewDidEndDragging(
    _ scrollView: UIScrollView,
    willDecelerate decelerate: Bool
)
```

## Parameters 

`scrollView`  

The scroll-view object that finished scrolling the content view.

`decelerate`  

true if the scrolling movement will continue, but decelerate, after a touch-up gesture during a dragging operation. If the value is false, scrolling stops immediately upon touch-up.

## Discussion

The scroll view sends this message when the user’s finger touches up after dragging content. The isDecelerating property of UIScrollView controls deceleration.

## See Also

### Responding to scrolling and dragging

func scrollViewDidScroll(UIScrollView)

Tells the delegate when the user scrolls the content view within the scroll view.

func scrollViewWillBeginDragging(UIScrollView)

Tells the delegate when the scroll view is about to start scrolling the content.

func scrollViewWillEndDragging(UIScrollView, withVelocity: CGPoint, targetContentOffset: UnsafeMutablePointer&lt;CGPoint>)

Tells the delegate when the user finishes scrolling the content.

func scrollViewShouldScrollToTop(UIScrollView) -> Bool

Asks the delegate if the scroll view should scroll to the top of the content.

func scrollViewDidScrollToTop(UIScrollView)

Tells the delegate that the scroll view scrolled to the top of the content.

func scrollViewWillBeginDecelerating(UIScrollView)

Tells the delegate that the scroll view is starting to decelerate the scrolling movement.

func scrollViewDidEndDecelerating(UIScrollView)

Tells the delegate that the scroll view ended decelerating the scrolling movement.

