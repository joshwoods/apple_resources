

- UIKit
- UIWebView
-  scrollView Deprecated

Instance Property

# scrollView

The scroll view associated with the web view.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0Deprecated

``` source
@MainActor
var scrollView: UIScrollView { get }
```

## Discussion

Your app can access the scroll view if it wants to customize the scrolling behavior of the web view.

## See Also

### Setting web content properties

var allowsLinkPreview: Bool

A Boolean value that determines whether pressing on a link displays a preview of the destination for the link.

Deprecated

var scalesPageToFit: Bool

A Boolean value determining whether the webpage scales to fit the view and the user can change the scale.

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

