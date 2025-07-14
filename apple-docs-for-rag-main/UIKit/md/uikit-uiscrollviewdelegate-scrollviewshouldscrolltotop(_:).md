

- UIKit
- UIScrollViewDelegate
-  scrollViewShouldScrollToTop(\_:) 

Instance Method

# scrollViewShouldScrollToTop(\_:)

Asks the delegate if the scroll view should scroll to the top of the content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewShouldScrollToTop(_ scrollView: UIScrollView) -> Bool
```

## Parameters 

`scrollView`  

The scroll-view object requesting this information.

## Return Value

true to permit scrolling to the top of the content, false to disallow it.

## Discussion

If the delegate doesn’t implement this method, true is assumed. For the scroll-to-top gesture (a tap on the status bar) to be effective, the scrollsToTop property of the UIScrollView must be set to true.

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

func scrollViewDidScrollToTop(UIScrollView)

Tells the delegate that the scroll view scrolled to the top of the content.

func scrollViewWillBeginDecelerating(UIScrollView)

Tells the delegate that the scroll view is starting to decelerate the scrolling movement.

func scrollViewDidEndDecelerating(UIScrollView)

Tells the delegate that the scroll view ended decelerating the scrolling movement.

