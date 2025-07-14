

- WebKit
- WKWebView
-  go(to:) 

Instance Method

# go(to:)

Navigates to an item from the back-forward list and sets it as the current item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func go(to item: WKBackForwardListItem) -> WKNavigation?
```

## Parameters 

`item`  

The item to navigate to. The item must be in the web view’s back-forward list.

## Return Value

A new navigation to the requested item, or `nil` if it is already the current item or is not part of the web view’s back-forward list.

## See Also

### Navigating between webpages

var allowsBackForwardNavigationGestures: Bool

A Boolean value that indicates whether horizontal swipe gestures trigger backward and forward page navigation.

var backForwardList: WKBackForwardList

The web view’s back-forward list.

func goBack(Any?)

Navigates to the back item in the back-forward list.

func goBack() -> WKNavigation?

Navigates to the back item in the back-forward list.

func goForward(Any?)

Navigates to the forward item in the back-forward list.

func goForward() -> WKNavigation?

Navigates to the forward item in the back-forward list.

var canGoBack: Bool

A Boolean value that indicates whether there is a valid back item in the back-forward list.

var canGoForward: Bool

A Boolean value that indicates whether there is a valid forward item in the back-forward list.

var allowsLinkPreview: Bool

A Boolean value that determines whether pressing a link displays a preview of the destination for the link.

var interactionState: Any?

An object you use to capture the current state of interaction in a web view so that you can restore that state later to another web view.

