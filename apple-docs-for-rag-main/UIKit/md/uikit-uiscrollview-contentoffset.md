

- UIKit
- UIScrollView
-  contentOffset 

Instance Property

# contentOffset

The point at which the origin of the content view is offset from the origin of the scroll view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentOffset: CGPoint { get set }
```

## Mentioned in 

Estimating the height of a table’s scrolling area

## Discussion

The default value is CGPointZero.

## See Also

### Managing the content size and offset

var contentSize: CGSize

The size of the content view.

func setContentOffset(CGPoint, animated: Bool)

Sets the offset from the content view’s origin that corresponds to the scroll view’s origin.

