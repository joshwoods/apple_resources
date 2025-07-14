

- Translation
- TranslationSession
- TranslationSession.Request
-  clientIdentifier 

Instance Property

# clientIdentifier

An optional unique identifier to associate a translation request with its response.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
var clientIdentifier: String?
```

## Discussion

When you set this identifier, it returns the same value in the corresponding TranslationSession.Response.

