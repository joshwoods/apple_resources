

- UIKit
- UIScrollViewDelegate
-  scrollViewDidScroll(\_:) 

Instance Method

# scrollViewDidScroll(\_:)

Tells the delegate when the user scrolls the content view within the scroll view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewDidScroll(_ scrollView: UIScrollView)
```

## Parameters 

`scrollView`  

The scroll-view object in which the scrolling occurred.

## Discussion

The delegate typically implements this method to obtain the change in content offset from `scrollView` and draw the affected portion of the content view.

## See Also

### Responding to scrolling and dragging

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

func scrollViewDidEndDecelerating(UIScrollView)

Tells the delegate that the scroll view ended decelerating the scrolling movement.

