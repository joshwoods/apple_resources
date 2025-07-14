

- WebKit
- WebBackForwardList
-  add(\_:) Deprecated

Instance Method

# add(\_:)

Inserts an item into the back-forward list, immediately after the current item.

macOS 10.4–10.14Deprecated

``` source
func add(_ item: WebHistoryItem!)
```

## Parameters 

`item`  

A web history item that represents a visited webpage. If `item` is `nil`, an invalidArgumentException exception is raised.

## Discussion

Any items following `item` in the back-forward list are removed. This method also removes items if the capacity of the receiver is exceeded.

