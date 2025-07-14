

- WebKit
- WebView
-  setMaintainsBackForwardList(\_:) Deprecated

Instance Method

# setMaintainsBackForwardList(\_:)

Sets whether to use a back-forward list.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func setMaintainsBackForwardList(_ flag: Bool)
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`flag`  

If false, clears the back-forward list and relinquishes ownership the page cache; otherwise, it does not.

## Discussion

The back-forward list maintains a page cache, so applications that do not use the goForward() or goBack() methods should disable it.

## See Also

### Moving Back and Forward

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

func go(toBackForwardItem: WebHistoryItem!) -> Bool

Loads a specific location from the back-forward list and sets it as the current item.

Deprecated

