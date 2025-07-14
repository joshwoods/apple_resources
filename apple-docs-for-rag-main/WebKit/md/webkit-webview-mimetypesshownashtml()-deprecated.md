

- WebKit
- WebView
-  mimeTypesShownAsHTML() Deprecated

Type Method

# mimeTypesShownAsHTML()

Returns a list of MIME types that WebKit renders as HTML.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class func mimeTypesShownAsHTML() -> [Any]!
```

Deprecated

No longer supported; please adopt WKWebView.

## Return Value

An array containing `NSString` objects that represent the MIME types WebKit attempts to render as HTML.

## See Also

### Getting and Setting Content Information

class func canShowMIMEType(String!) -> Bool

Returns whether the receiver can display content of a given MIME type.

Deprecated

class func setMIMETypesShownAsHTML([Any]!)

Sets the MIME types that WebKit attempts to render as HTML.

Deprecated

class func canShowMIMEType(asHTML: String!) -> Bool

Returns whether the receiver interprets a MIME type as HTML.

Deprecated

var supportsTextEncoding: Bool

A Boolean that indicates whether the document view supports different text encodings.

Deprecated

var customTextEncodingName: String!

The custom text encoding name.

Deprecated

var textSizeMultiplier: Float

The font size multiplier for text displayed in web frame view objects managed by the receiver.

Deprecated

