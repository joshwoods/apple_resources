

- WebKit
- WebBackForwardList
-  item(at:) Deprecated

Instance Method

# item(at:)

Returns the item at the specified index in the back-forward list.

macOS 10.4–10.14Deprecated

``` source
func item(at index: Int32) -> WebHistoryItem!
```

## Parameters 

`index`  

The index of the item to return. The position of the current item is index `0`, and the position of any other item is expressed as an offset from index `0`. For example, the item preceding the current item is at index `-1`, and the item following the current item is at index `1`.

## Return Value

The item at the specified index, or `nil` if `index` exceeds the bounds of the back-forward list (that is, if `index` is greater than the value returned by forwardListCount, or less than the negative form of the value returned by backListCount).

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

var forwardItem: WebHistoryItem!

The item that follows the current item in the back-forward list.

Deprecated

var forwardListCount: Int32

The number of items that follow the current item in the back-forward list.

Deprecated

func forwardList(withLimit: Int32) -> [Any]!

Returns the items that follow the current item in the back-forward list, up to the specified number of items.

Deprecated

