

- WebKit
- WebBackForwardList
-  forwardList(withLimit:) Deprecated

Instance Method

# forwardList(withLimit:)

Returns the items that follow the current item in the back-forward list, up to the specified number of items.

macOS 10.4–10.14Deprecated

``` source
func forwardList(withLimit limit: Int32) -> [Any]!
```

## Parameters 

`limit`  

The greatest number of items to return.

## Return Value

An array containing (at most) the specified number of items, or `nil` if no items follow the current item.

## See Also

### Querying the Back-Forward List

var backItem: WebHistoryItem!

The item that precedes the current item in the back-forward list.

Deprecated

var backListCount: Int32

The number of items that precede the current item in the back-forward list.

Deprecated

func back(withLimit: Int32) -> [Any]!

Returns the items that precede the current item in the back-forward list, up to the specified number of items.

Deprecated

func contains(WebHistoryItem!) -> Bool

Returns a Boolean value indicating whether the back-forward list contains the specified item.

Deprecated

var currentItem: WebHistoryItem!

The current item in the back-forward list.

Deprecated

func item(at: Int32) -> WebHistoryItem!

Returns the item at the specified index in the back-forward list.

Deprecated

var forwardItem: WebHistoryItem!

The item that follows the current item in the back-forward list.

Deprecated

var forwardListCount: Int32

The number of items that follow the current item in the back-forward list.

Deprecated

