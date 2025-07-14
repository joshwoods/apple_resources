

- UIKit
- UIWebView
-  keyboardDisplayRequiresUserAction Deprecated

Instance Property

# keyboardDisplayRequiresUserAction

A Boolean value indicating whether web content can programmatically display the keyboard.

iOS 6.0–12.0DeprecatediPadOS 6.0–12.0Deprecated

``` source
@MainActor
var keyboardDisplayRequiresUserAction: Bool { get set }
```

## Discussion

When this property is set to true, the user must explicitly tap the elements in the web view to display the keyboard (or other relevant input view) for that element. When set to false, a focus event on an element causes the input view to be displayed and associated with that element automatically.

The default value for this property is true.

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

var dataDetectorTypes: UIDataDetectorTypes

The types of data converted to clickable URLs in the web view’s content.

Deprecated

