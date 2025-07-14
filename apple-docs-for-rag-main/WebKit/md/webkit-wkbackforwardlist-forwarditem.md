

- WebKit
- WKBackForwardList
-  forwardItem 

Instance Property

# forwardItem

The item immediately following the current item, if any.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var forwardItem: WKBackForwardListItem? { get }
```

## Discussion

If the current item is the last item in the list, this value in this property is `nil`.

## See Also

### Getting the Most Recent Items

var backItem: WKBackForwardListItem?

The item immediately preceding the current item, if any.

var currentItem: WKBackForwardListItem?

The current item.

