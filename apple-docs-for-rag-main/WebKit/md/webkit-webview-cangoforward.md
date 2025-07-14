

- WebKit
- WebView
-  canGoForward 

Instance Property

# canGoForward

A Boolean that indicates whether the next location can be loaded.

macOS

``` source
@MainActor
var canGoForward: Bool { get }
```

## Discussion

true if able to move forward; otherwise, false.

## See Also

### Moving Back and Forward

func setMaintainsBackForwardList(Bool)

Sets whether to use a back-forward list.

Deprecated

var backForwardList: WebBackForwardList!

The receiver’s back-forward list.

Deprecated

var canGoBack: Bool

A Boolean that indicates whether the previous location can be loaded.

func goBack() -> Bool

Loads the previous location in the back-forward list.

Deprecated

func goBack(Any?)

An action method that loads the previous location in the back-forward list.

func goForward() -> Bool

Loads the next location in the back-forward list.

Deprecated

func goForward(Any?)

An action method that loads the next location in the back-forward list.

func go(toBackForwardItem: WebHistoryItem!) -> Bool

Loads a specific location from the back-forward list and sets it as the current item.

Deprecated

