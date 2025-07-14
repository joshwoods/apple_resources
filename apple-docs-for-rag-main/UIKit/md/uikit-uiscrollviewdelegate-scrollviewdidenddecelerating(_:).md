

- UIKit
- UIScrollViewDelegate
-  scrollViewDidEndDecelerating(\_:) 

Instance Method

# scrollViewDidEndDecelerating(\_:)

Tells the delegate that the scroll view ended decelerating the scrolling movement.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewDidEndDecelerating(_ scrollView: UIScrollView)
```

## Parameters 

`scrollView`  

The scroll-view object that’s decelerating the scrolling of the content view.

## Discussion

The scroll view calls this method when the scrolling movement comes to a halt. The isDecelerating property of `UIScrollView` controls deceleration.

## See Also

### Responding to scrolling and dragging

func scrollViewDidScroll(UIScrollView)

Tells the delegate when the user scrolls the content view within the scroll view.

func scrollViewWillBeginDragging(UIScrollView)

Tells the delegate when the scroll view is about to start scrolling the content.

func scrollViewWillEndDragging(UIScrollView, withVelocity: CGPoint, targetContentOffset: UnsafeMutablePointer&lt;CGPoint>)

Tells the delegate when the user finishes scrolling the content.

func scrollViewDidEndDragging(UIScrollView, willDecelerate: Bool)

Tells the delegate when dragging ended in the scroll view.

func scrollViewShouldScrollToTop(UIScrollView) -> Bool

Asks the delegate if the scroll view should scroll to the top of the content.

func scrollViewDidScrollToTop(UIScrollView)

Tells the delegate that the scroll view scrolled to the top of the content.

func scrollViewWillBeginDecelerating(UIScrollView)

Tells the delegate that the scroll view is starting to decelerate the scrolling movement.

