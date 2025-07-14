

- WebKit
- WebView
-  backForwardList Deprecated

Instance Property

# backForwardList

The receiver’s back-forward list.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var backForwardList: WebBackForwardList! { get }
```

Deprecated

No longer supported; please adopt WKWebView.

## See Also

### Moving Back and Forward

func setMaintainsBackForwardList(Bool)

Sets whether to use a back-forward list.

Deprecated

var canGoBack: Bool

A Boolean that indicates whether the previous location can be loaded.

func goBack() -> Bool

Loads the previous location in the back-forward list.

Deprecated

func goBack(Any?)

An action method that loads the previous location in the back-forward list.

var canGoForward: Bool

A Boolean that indicates whether the next location can be loaded.

func goForward() -> Bool

Loads the next location in the back-forward list.

Deprecated

func goForward(Any?)

An action method that loads the next location in the back-forward list.

func go(toBackForwardItem: WebHistoryItem!) -> Bool

Loads a specific location from the back-forward list and sets it as the current item.

Deprecated

