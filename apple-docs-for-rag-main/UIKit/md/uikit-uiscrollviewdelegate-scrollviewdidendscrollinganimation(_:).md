

- UIKit
- UIScrollViewDelegate
-  scrollViewDidEndScrollingAnimation(\_:) 

Instance Method

# scrollViewDidEndScrollingAnimation(\_:)

Tells the delegate when a scrolling animation in the scroll view concludes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func scrollViewDidEndScrollingAnimation(_ scrollView: UIScrollView)
```

## Parameters 

`scrollView`  

The scroll-view object that’s performing the scrolling animation.

## Discussion

The scroll view calls this method at the end of its implementations of the setContentOffset(_:animated:) and scrollRectToVisible(_:animated:) methods, but only if animations are requested.

