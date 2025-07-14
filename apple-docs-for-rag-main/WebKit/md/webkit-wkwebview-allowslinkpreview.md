

- WebKit
- WKWebView
-  allowsLinkPreview 

Instance Property

# allowsLinkPreview

A Boolean value that determines whether pressing a link displays a preview of the destination for the link.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
var allowsLinkPreview: Bool { get set }
```

## Discussion

In iOS, this property is available on devices that support 3D Touch. In iOS 10 and later, the default value is true; in previous versions of iOS, the default value is false.

If you set this property’s value to true, an iOS user can press links to preview link destinations and detected data such as addresses and phone numbers. Such previews are known to users as *peeks*. If a user presses deeper on a link preview, the preview navigates (or *pops*, in user terminology) to the destination. Because pop navigation switches the user from your app to Safari, it is opt-in for iOS apps.

If you want to support link preview in iOS but also want to keep users within your app, you can switch from using the WKWebView class to the SFSafariViewController class. If you are using a web view as an in-app browser, making this change is best practice. The Safari view controller class automatically supports link previews.

In macOS, this property is available on devices with a Force Touch trackpad. The default value is true.

With this property set to its default value of true, a macOS user can force click a link to display a preview window showing the link’s destination. If the user then clicks the preview, the destination opens in Safari.

On both platforms, all types of detected data respond to presses when this property is set to true. That is, in iOS 9 and OS X 10.11, you cannot specify which types of data are detected in the WKWebView class.

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

func go(to: WKBackForwardListItem) -> WKNavigation?

Navigates to an item from the back-forward list and sets it as the current item.

var canGoBack: Bool

A Boolean value that indicates whether there is a valid back item in the back-forward list.

var canGoForward: Bool

A Boolean value that indicates whether there is a valid forward item in the back-forward list.

var interactionState: Any?

An object you use to capture the current state of interaction in a web view so that you can restore that state later to another web view.

