

- Authentication Services
- ASWebAuthenticationSession
-  ASWebAuthenticationSession.CompletionHandler 

Type Alias

# ASWebAuthenticationSession.CompletionHandler

A completion handler for the web authentication session.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CompletionHandler = (URL?, (any Error)?) -> Void
```

## See Also

### Creating a Session

init(url: URL, callbackURLScheme: String?, completionHandler: ASWebAuthenticationSession.CompletionHandler)

Creates a web authentication session instance.

Deprecated

