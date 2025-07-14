

- Translation
- TranslationSession
- TranslationSession.Response
-  clientIdentifier 

Instance Property

# clientIdentifier

The unique identifier matching the client identifier set in the translation request.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
let clientIdentifier: String?
```

## Discussion

Use this identifier to associate a translation request with its response. If you set a client identifier in the translation request, that same identifier returns in the response. If the request contained no identifier, this value is `nil`.

