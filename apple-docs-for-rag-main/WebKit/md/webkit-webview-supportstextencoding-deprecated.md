

- WebKit
- WebView
-  supportsTextEncoding Deprecated

Instance Property

# supportsTextEncoding

A Boolean that indicates whether the document view supports different text encodings.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var supportsTextEncoding: Bool { get }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

true if the receiver’s document view can support different text encodings; otherwise, false.

## See Also

### Getting and Setting Content Information

class func canShowMIMEType(String!) -> Bool

Returns whether the receiver can display content of a given MIME type.

Deprecated

class func mimeTypesShownAsHTML() -> [Any]!

Returns a list of MIME types that WebKit renders as HTML.

Deprecated

class func setMIMETypesShownAsHTML([Any]!)

Sets the MIME types that WebKit attempts to render as HTML.

Deprecated

class func canShowMIMEType(asHTML: String!) -> Bool

Returns whether the receiver interprets a MIME type as HTML.

Deprecated

var customTextEncodingName: String!

The custom text encoding name.

Deprecated

var textSizeMultiplier: Float

The font size multiplier for text displayed in web frame view objects managed by the receiver.

Deprecated

