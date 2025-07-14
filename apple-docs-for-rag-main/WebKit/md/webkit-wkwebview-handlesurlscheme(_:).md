

- WebKit
- WKWebView
-  handlesURLScheme(\_:) 

Type Method

# handlesURLScheme(\_:)

Returns a Boolean value that indicates whether WebKit natively supports resources with the specified URL scheme.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
class func handlesURLScheme(_ urlScheme: String) -> Bool
```

## Parameters 

`urlScheme`  

The URL scheme associated with the resource.

## Return Value

true if WebKit provides native support for the URL scheme, or false if it doesn’t.

