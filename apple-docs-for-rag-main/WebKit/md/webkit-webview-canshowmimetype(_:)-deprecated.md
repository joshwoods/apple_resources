

- WebKit
- WebView
-  canShowMIMEType(\_:) Deprecated

Type Method

# canShowMIMEType(\_:)

Returns whether the receiver can display content of a given MIME type.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class func canShowMIMEType(_ MIMEType: String!) -> Bool
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`MIMEType`  

The MIME type of the content.

## Return Value

true if the receiver can display content of the specified MIME type where `MIMEType` is one of the standard types like “image/gif”; otherwise, false.

## See Also

### Getting and Setting Content Information

class func mimeTypesShownAsHTML() -> [Any]!

Returns a list of MIME types that WebKit renders as HTML.

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

