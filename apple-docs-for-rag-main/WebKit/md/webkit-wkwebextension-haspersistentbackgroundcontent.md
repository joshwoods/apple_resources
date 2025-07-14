

- WebKit
- WKWebExtension
-  hasPersistentBackgroundContent 

Instance Property

# hasPersistentBackgroundContent

A Boolean value indicating whether the extension has background content that stays in memory as long as the extension is loaded.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasPersistentBackgroundContent: Bool { get }
```

## Discussion

Note

Note that extensions are only allowed to have persistent background content on macOS. An WKWebExtension.Error.Code.invalidBackgroundPersistence error will be reported on iOS, iPadOS, and visionOS if an attempt is made to load a persistent extension.

