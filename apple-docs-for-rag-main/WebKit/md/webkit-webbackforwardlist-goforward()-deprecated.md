

- WebKit
- WebBackForwardList
-  goForward() Deprecated

Instance Method

# goForward()

Moves forward one item in the back-forward list.

macOS 10.4–10.14Deprecated

``` source
func goForward()
```

## Discussion

This method works by changing the current item to the item that follows it. This method raises an internalInconsistencyException exception if no item follows the current item.

## See Also

### Moving Backward and Forward

func goBack()

Moves backward one item in the back-forward list.

Deprecated

func go(to: WebHistoryItem!)

Makes the specified item in the back-forward list the current item.

Deprecated

