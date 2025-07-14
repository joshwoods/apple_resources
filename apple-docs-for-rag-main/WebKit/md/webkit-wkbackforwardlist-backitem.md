

- WebKit
- WKBackForwardList
-  backItem 

Instance Property

# backItem

The item immediately preceding the current item, if any.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var backItem: WKBackForwardListItem? { get }
```

## Discussion

If the current item is the first item in the list, the value in this property is `nil`.

## See Also

### Getting the Most Recent Items

var currentItem: WKBackForwardListItem?

The current item.

var forwardItem: WKBackForwardListItem?

The item immediately following the current item, if any.

