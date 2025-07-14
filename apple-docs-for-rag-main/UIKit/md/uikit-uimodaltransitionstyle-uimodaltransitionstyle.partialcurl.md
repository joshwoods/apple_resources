

- UIKit
- UIModalTransitionStyle
-  UIModalTransitionStyle.partialCurl 

Case

# UIModalTransitionStyle.partialCurl

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
case partialCurl
```

## Discussion

When the view controller is presented, one corner of the current view curls up to reveal the presented view underneath. On dismissal, the curled up page unfurls itself back on top of the presented view. A view controller presented using this transition is itself prevented from presenting any additional view controllers.

This transition style is supported only if the parent view controller is presenting a full-screen view and you use the UIModalPresentationStyle.fullScreen modal presentation style. Attempting to use a different form factor for the parent view or a different presentation style triggers an exception.

## See Also

### Constants

case coverVertical

case flipHorizontal

case crossDissolve

