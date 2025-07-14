

- UIKit
- UIWebView
-  scalesPageToFit Deprecated

Instance Property

# scalesPageToFit

A Boolean value determining whether the webpage scales to fit the view and the user can change the scale.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
var scalesPageToFit: Bool { get set }
```

## Discussion

If true, the webpage is scaled to fit and the user can zoom in and zoom out. If false, user zooming is disabled. The default value is false.

## See Also

### Setting web content properties

var allowsLinkPreview: Bool

A Boolean value that determines whether pressing on a link displays a preview of the destination for the link.

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

