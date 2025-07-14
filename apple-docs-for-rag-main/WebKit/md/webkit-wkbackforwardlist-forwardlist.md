

- WebKit
- WKBackForwardList
-  forwardList 

Instance Property

# forwardList

The array of items that follow the current item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var forwardList: [WKBackForwardListItem] { get }
```

## Discussion

The items are in the order in which the web view originally visited them.

## See Also

### Getting Sublists

var backList: [WKBackForwardListItem]

The array of items that precede the current item.

