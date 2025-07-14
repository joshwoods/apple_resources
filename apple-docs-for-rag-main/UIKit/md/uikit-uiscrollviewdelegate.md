

- UIKit
-  UIScrollViewDelegate 

Protocol

# UIScrollViewDelegate

The interface for the delegate of a scroll view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIScrollViewDelegate : NSObjectProtocol
```

## Overview

The methods that the UIScrollViewDelegate protocol declares allow the adopting delegate to respond to messages from the UIScrollView class. The delegate responds to and affects operations like scrolling, zooming, deceleration of scrolled content, and scrolling animations.

## Topics

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

func scrollViewDidEndDecelerating(UIScrollView)

Tells the delegate that the scroll view ended decelerating the scrolling movement.

### Managing zooming

func viewForZooming(in: UIScrollView) -> UIView?

Asks the delegate for the view to scale when zooming is about to occur in the scroll view.

func scrollViewWillBeginZooming(UIScrollView, with: UIView?)

Tells the delegate that zooming of the content in the scroll view is about to commence.

func scrollViewDidEndZooming(UIScrollView, with: UIView?, atScale: CGFloat)

Tells the delegate when zooming of the content in the scroll view completed.

func scrollViewDidZoom(UIScrollView)

Tells the delegate that the scroll view’s zoom factor changed.

### Responding to scrolling animations

func scrollViewDidEndScrollingAnimation(UIScrollView)

Tells the delegate when a scrolling animation in the scroll view concludes.

### Responding to inset changes

func scrollViewDidChangeAdjustedContentInset(UIScrollView)

Tells the delegate when the scroll view’s inset values change.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UICollectionViewDelegate
- UICollectionViewDelegateFlowLayout
- UIScrollViewAccessibilityDelegate
- UITableViewDelegate
- UITextViewDelegate

### Conforming Types

- UICollectionViewController
- UITableViewController
- UIWebView

## See Also

### Responding to scroll view interactions

var delegate: (any UIScrollViewDelegate)?

The delegate of the scroll view.

