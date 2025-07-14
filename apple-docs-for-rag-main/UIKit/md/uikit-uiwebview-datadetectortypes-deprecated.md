

- UIKit
- UIWebView
-  dataDetectorTypes Deprecated

Instance Property

# dataDetectorTypes

The types of data converted to clickable URLs in the web view’s content.

iOS 3.0–12.0DeprecatediPadOS 3.0–12.0Deprecated

``` source
@MainActor
var dataDetectorTypes: UIDataDetectorTypes { get set }
```

## Discussion

Use this property to specify the types of data (phone numbers, HTTP links, email address, and so on) that should be automatically converted to clickable URLs in the web view. When clicked, the web view opens the app responsible for handling the URL type and passes it the URL.

See the UIDataDetectorTypes enumeration for the types of data available for automatic detection.

## See Also

### Setting web content properties

var allowsLinkPreview: Bool

A Boolean value that determines whether pressing on a link displays a preview of the destination for the link.

Deprecated

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

