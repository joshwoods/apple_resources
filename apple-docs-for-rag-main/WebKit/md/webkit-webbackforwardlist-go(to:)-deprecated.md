

- WebKit
- WebBackForwardList
-  go(to:) Deprecated

Instance Method

# go(to:)

Makes the specified item in the back-forward list the current item.

macOS 10.4–10.14Deprecated

``` source
func go(to item: WebHistoryItem!)
```

## Parameters 

`item`  

A web history item that represents a visited webpage. If `item` is not in the back-forward list, an invalidArgumentException exception is raised.

## See Also

### Moving Backward and Forward

func goBack()

Moves backward one item in the back-forward list.

Deprecated

func goForward()

Moves forward one item in the back-forward list.

Deprecated

