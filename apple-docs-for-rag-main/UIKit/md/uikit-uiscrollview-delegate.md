

- UIKit
- UIScrollView
-  delegate 

Instance Property

# delegate

The delegate of the scroll view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIScrollViewDelegate)? { get set }
```

## Discussion

The delegate must adopt the UIScrollViewDelegate protocol. The UIScrollView class, which doesn’t retain the delegate, invokes each protocol method the delegate implements.

## See Also

### Responding to scroll view interactions

protocol UIScrollViewDelegate

The interface for the delegate of a scroll view.

