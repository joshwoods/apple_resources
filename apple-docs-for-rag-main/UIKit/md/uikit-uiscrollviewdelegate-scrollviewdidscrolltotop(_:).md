

- UIKit
- UIScrollViewDelegate
-  scrollViewDidScrollToTop(\_:) 

Instance Method

# scrollViewDidScrollToTop(\_:)

Tells the delegate that the scroll view scrolled to the top of the content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewDidScrollToTop(_ scrollView: UIScrollView)
```

## Parameters 

`scrollView`  

The scroll-view object that perform the scrolling operation.

## Discussion

The scroll view sends this message when it finishes scrolling to the top of the content. It might call it immediately if the top of the content is already shown. For the scroll-to-top gesture (a tap on the status bar) to be effective, the scrollsToTop property of the UIScrollView must be set to true.

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

func scrollViewWillBeginDecelerating(UIScrollView)

Tells the delegate that the scroll view is starting to decelerate the scrolling movement.

func scrollViewDidEndDecelerating(UIScrollView)

Tells the delegate that the scroll view ended decelerating the scrolling movement.

