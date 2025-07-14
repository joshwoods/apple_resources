

- UIKit
- UIFocusItemScrollableContainer
-  contentSize 

Instance Property

# contentSize

The total size of the content contained by this container.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
var contentSize: CGSize { get }
```

**Required**

## Discussion

If the value of this property is larger than visibleSize then the content is scrollable.

## See Also

### Retrieving the content size

var contentOffset: CGPoint

The current content offset for the scrollable container.

**Required**

var visibleSize: CGSize

The visible size of the scrollable container.

**Required**

