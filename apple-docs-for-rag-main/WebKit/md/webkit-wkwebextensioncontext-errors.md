

- WebKit
- WKWebExtensionContext
-  errors 

Instance Property

# errors

All errors that occurred in the extension context.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var errors: [any Error] { get }
```

## Discussion

Provides an array of all parse-time and runtime errors for the extension and extension context, with repeat errors consolidated into a single entry for the original occurrence. If no errors occurred, an empty array is returned.

