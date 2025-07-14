

- WebKit
- WebBackForwardList
-  goBack() Deprecated

Instance Method

# goBack()

Moves backward one item in the back-forward list.

macOS 10.4–10.14Deprecated

``` source
func goBack()
```

## Discussion

This method works by changing the current item to the item that precedes it. This method raises an internalInconsistencyException exception if no item precedes the current item.

## See Also

### Moving Backward and Forward

func goForward()

Moves forward one item in the back-forward list.

Deprecated

func go(to: WebHistoryItem!)

Makes the specified item in the back-forward list the current item.

Deprecated

