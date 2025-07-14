

- WebKit
- WebView
-  registerURLScheme(asLocal:) Deprecated

Type Method

# registerURLScheme(asLocal:)

Adds the specified URL scheme to the list of local schemes.

macOS 10.3–10.14Deprecated

``` source
@MainActor
class func registerURLScheme(asLocal scheme: String!)
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`scheme`  

The scheme to add to the list.

## Discussion

You need to register a scheme as local to access resources with file URLs and to have the same security checks as a local file.

## See Also

### Registering Document Views and Representations

class func registerClass(AnyClass!, representationClass: AnyClass!, forMIMEType: String!)

Specifies the view and representation objects to be used for specific MIME types.

Deprecated

