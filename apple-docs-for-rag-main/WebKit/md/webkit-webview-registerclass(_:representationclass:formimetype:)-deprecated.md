

- WebKit
- WebView
-  registerClass(\_:representationClass:forMIMEType:) Deprecated

Type Method

# registerClass(\_:representationClass:forMIMEType:)

Specifies the view and representation objects to be used for specific MIME types.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class func registerClass(
    _ viewClass: AnyClass!,
    representationClass: AnyClass!,
    forMIMEType MIMEType: String!
)
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`viewClass`  

A class conforming to the WebDocumentView protocol that displays the specified MIME types.

`representationClass`  

The class conforming to WebDocumentRepresentation protocol that represents the specified MIME types.

`MIMEType`  

The MIME type of the content.

This may be a primary MIME type or subtype. For example, if `MIMEType` is “video/” the specified view and representation objects are used for all video types. More specific subtype mappings, such as “image/gif”, takes precedence over primary type matching, such as “image/”.

## Discussion

After invoking this method, when `MIMEType` content is encountered, instances of `representationClass` and `viewClass` are created to handle and display it.

## See Also

### Registering Document Views and Representations

class func registerURLScheme(asLocal: String!)

Adds the specified URL scheme to the list of local schemes.

Deprecated

