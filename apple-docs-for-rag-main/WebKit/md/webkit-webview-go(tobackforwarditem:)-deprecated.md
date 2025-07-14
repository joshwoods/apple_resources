

- WebKit
- WebView
-  go(toBackForwardItem:) Deprecated

Instance Method

# go(toBackForwardItem:)

Loads a specific location from the back-forward list and sets it as the current item.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func go(toBackForwardItem item: WebHistoryItem!) -> Bool
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`item`  

The index of the location to load. This method sets the current item in the back-forward list to `item`.

## Return Value

true if `item` is in the back-forward list; otherwise, false.

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

var canGoForward: Bool

A Boolean that indicates whether the next location can be loaded.

func goForward() -> Bool

Loads the next location in the back-forward list.

Deprecated

func goForward(Any?)

An action method that loads the next location in the back-forward list.

