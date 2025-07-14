

- UIKit
- UIWebView
-  suppressesIncrementalRendering Deprecated

Instance Property

# suppressesIncrementalRendering

A Boolean value indicating whether the web view suppresses content rendering until it is fully loaded into memory.

iOS 6.0–12.0DeprecatediPadOS 6.0–12.0Deprecated

``` source
@MainActor
var suppressesIncrementalRendering: Bool { get set }
```

## Discussion

When set to true, the web view does not attempt to render incoming content as it arrives. Instead, the view’s current contents remain in place until all of the new content has been received, at which point the new content is rendered. This property does not affect the rendering of content retrieved after a frame finishes loading.

The value of this property is false by default.

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

var keyboardDisplayRequiresUserAction: Bool

A Boolean value indicating whether web content can programmatically display the keyboard.

Deprecated

var dataDetectorTypes: UIDataDetectorTypes

The types of data converted to clickable URLs in the web view’s content.

Deprecated

