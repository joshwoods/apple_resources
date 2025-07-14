

- WebKit
- WKWebView
-  goBack(\_:) 

Instance Method

# goBack(\_:)

Navigates to the back item in the back-forward list.

macOS

``` source
@IBAction @MainActor
func goBack(_ sender: Any?)
```

## Parameters 

`sender`  

The object sending this message.

## See Also

### Navigating between webpages

var allowsBackForwardNavigationGestures: Bool

A Boolean value that indicates whether horizontal swipe gestures trigger backward and forward page navigation.

var backForwardList: WKBackForwardList

The web view’s back-forward list.

func goBack() -> WKNavigation?

Navigates to the back item in the back-forward list.

func goForward(Any?)

Navigates to the forward item in the back-forward list.

func goForward() -> WKNavigation?

Navigates to the forward item in the back-forward list.

func go(to: WKBackForwardListItem) -> WKNavigation?

Navigates to an item from the back-forward list and sets it as the current item.

var canGoBack: Bool

A Boolean value that indicates whether there is a valid back item in the back-forward list.

var canGoForward: Bool

A Boolean value that indicates whether there is a valid forward item in the back-forward list.

var allowsLinkPreview: Bool

A Boolean value that determines whether pressing a link displays a preview of the destination for the link.

var interactionState: Any?

An object you use to capture the current state of interaction in a web view so that you can restore that state later to another web view.

