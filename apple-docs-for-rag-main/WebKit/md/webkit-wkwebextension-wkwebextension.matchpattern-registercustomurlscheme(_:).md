

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  registerCustomURLScheme(\_:) 

Type Method

# registerCustomURLScheme(\_:)

Registers a custom URL scheme that can be used in match patterns.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class func registerCustomURLScheme(_ urlScheme: String)
```

## Parameters 

`urlScheme`  

The custom URL scheme to register.

## Discussion

This method should be used to register any custom URL schemes used by the app for the extension base URLs, other than `webkit-extension`, or if extensions should have access to other supported URL schemes when using ``.

