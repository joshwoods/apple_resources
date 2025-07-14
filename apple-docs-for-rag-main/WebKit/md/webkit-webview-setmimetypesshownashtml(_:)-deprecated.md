

- WebKit
- WebView
-  setMIMETypesShownAsHTML(\_:) Deprecated

Type Method

# setMIMETypesShownAsHTML(\_:)

Sets the MIME types that WebKit attempts to render as HTML.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class func setMIMETypesShownAsHTML(_ MIMETypes: [Any]!)
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`MIMETypes`  

An array of `NSString` objects representing the MIME types. Typically, you create the `MIMETypes` array by adding additional types to the array returned by the mimeTypesShownAsHTML() class method.

## See Also

### Getting and Setting Content Information

class func canShowMIMEType(String!) -> Bool

Returns whether the receiver can display content of a given MIME type.

Deprecated

class func mimeTypesShownAsHTML() -> [Any]!

Returns a list of MIME types that WebKit renders as HTML.

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

