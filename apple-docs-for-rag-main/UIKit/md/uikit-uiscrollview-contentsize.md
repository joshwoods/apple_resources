

- UIKit
- UIScrollView
-  contentSize 

Instance Property

# contentSize

The size of the content view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentSize: CGSize { get set }
```

## Mentioned in 

Estimating the height of a table’s scrolling area

## Discussion

The unit of size is points. The default size is CGSizeZero.

## See Also

### Managing the content size and offset

var contentOffset: CGPoint

The point at which the origin of the content view is offset from the origin of the scroll view.

func setContentOffset(CGPoint, animated: Bool)

Sets the offset from the content view’s origin that corresponds to the scroll view’s origin.

