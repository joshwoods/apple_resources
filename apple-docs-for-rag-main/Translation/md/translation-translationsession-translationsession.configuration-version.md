

- Translation
- TranslationSession
- TranslationSession.Configuration
-  version 

Instance Property

# version

A value the equals function uses to represent change in the configuration instance.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
var version: Int { get }
```

## Discussion

This integer changes when you call invalidate() on an instance of your translation session.

