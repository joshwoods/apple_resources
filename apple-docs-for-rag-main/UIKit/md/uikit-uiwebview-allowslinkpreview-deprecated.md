

- UIKit
- UIWebView
-  allowsLinkPreview Deprecated

Instance Property

# allowsLinkPreview

A Boolean value that determines whether pressing on a link displays a preview of the destination for the link.

iOS 9.0–12.0DeprecatediPadOS 9.0–12.0Deprecated

``` source
@MainActor
var allowsLinkPreview: Bool { get set }
```

## Discussion

This property is available on devices that support 3D Touch. Default value is false.

If you set this value to true for a web view, users (with devices that support 3D Touch) can preview link destinations, and can preview detected data such as addresses, by pressing on links. Such previews are known to users as *peeks*. If a user presses deeper, the preview navigates (or *pops*, in user terminology) to the destination. Because pop navigation switches the user from your app to Safari, it is opt-in, by way of this property, rather default behavior for this class.

If you want to support link preview but also want to keep users within your app, you can switch from using the UIWebView class to the SFSafariViewController class. If you are using a web view as an in-app browser, making this change is best practice. The Safari view controller class automatically supports link previews.

## See Also

### Setting web content properties

var scalesPageToFit: Bool

A Boolean value determining whether the webpage scales to fit the view and the user can change the scale.

Deprecated

var scrollView: UIScrollView

The scroll view associated with the web view.

Deprecated

var suppressesIncrementalRendering: Bool

A Boolean value indicating whether the web view suppresses content rendering until it is fully loaded into memory.

Deprecated

var keyboardDisplayRequiresUserAction: Bool

A Boolean value indicating whether web content can programmatically display the keyboard.

Deprecated

var dataDetectorTypes: UIDataDetectorTypes

The types of data converted to clickable URLs in the web view’s content.

Deprecated

