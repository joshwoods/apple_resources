

- UIKit
- UIScrollView
-  transfersVerticalScrollingToParent 

Instance Property

# transfersVerticalScrollingToParent

A Boolean value that determines whether the scroll view passes vertical scroll events to a superview.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
var transfersVerticalScrollingToParent: Bool { get set }
```

## Discussion

The default value is `true`, in which case when the scroll view reaches either end of its vertical scroll axis it transfers scroll events to a containing scroll view. To stop this behavior, set the property to `false`.

## See Also

### Nesting scroll views

var transfersHorizontalScrollingToParent: Bool

A Boolean value that determines whether the scroll view passes horizontal scroll events to a superview.

