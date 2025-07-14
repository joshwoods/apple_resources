

- WebKit
-  WebFrameView Deprecated

Class

# WebFrameView

`WebFrameView` objects and their subviews display the web content contained in a frame. You never create instances of `WebFrameView` directly—`WebView` objects create and manage a hierarchy of `WebFrameView` objects, one for each frame. `WebFrameView` objects use a scroll view whose document view conforms to the WebDocumentView protocol.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class WebFrameView
```

## Topics

### Getting the Web Frame

var webFrame: WebFrame!

The web frame.

### Getting Subviews

var documentView: (any NSView &amp; WebDocumentView)!

The subview that displays the web content.

### Setting Scrolling Behavior

var allowsScrolling: Bool

A Boolean that indicates whether the frame view should allow users to scroll.

### Printing Views

var canPrintHeadersAndFooters: Bool

A Boolean value indicating whether the receiver can print headers and footers.

func printOperation(with: NSPrintInfo!) -> NSPrintOperation!

Returns a print operation object to print this frame.

var documentViewShouldHandlePrint: Bool

A Boolean value indicating whether the document view should handle a print operation.

func printDocumentView()

Prints the receiver.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Working with Frames (Legacy)

class WebFrame

A `WebFrame` object encapsulates the data displayed in a `WebFrameView` object. There is one `WebFrame` object per frame displayed in a `WebView`. An entire webpage is represented by a hierarchy of `WebFrame` objects in which the root object is called the **main frame**.

Deprecated

class WebDataSource

`WebDataSource` encapsulates the web content to be displayed in a web frame view. A `WebDataSource` object has a representation object, conforming to the `WebDocumentRepresentation` protocol, that holds the data in an appropriate format depending on the MIME type. You can extend WebKit to support new MIME types by implementing your own view and representation classes, and specifying the mapping between them using the registerClass(_:representationClass:forMIMEType:) `WebView` class method.

Deprecated

protocol WebFrameLoadDelegateDeprecated

