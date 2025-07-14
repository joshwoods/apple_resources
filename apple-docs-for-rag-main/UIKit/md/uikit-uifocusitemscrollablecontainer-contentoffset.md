

- UIKit
- UIFocusItemScrollableContainer
-  contentOffset 

Instance Property

# contentOffset

The current content offset for the scrollable container.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
var contentOffset: CGPoint { get set }
```

**Required**

## Discussion

If the scrollable container contains `bounds`, then `bounds.origin` must be equal to the content offset. The system repeatedly sets this property to simulate animated scrolling.

## See Also

### Retrieving the content size

var contentSize: CGSize

The total size of the content contained by this container.

**Required**

var visibleSize: CGSize

The visible size of the scrollable container.

**Required**

