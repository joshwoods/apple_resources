

- WebKit
- WKWebExtensionContext
-  hasRequestedOptionalAccessToAllHosts 

Instance Property

# hasRequestedOptionalAccessToAllHosts

A Boolean value indicating if the extension has requested optional access to all hosts.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasRequestedOptionalAccessToAllHosts: Bool { get set }
```

## Discussion

If this property is `YES`, the extension has asked for access to all hosts in a call to `browser.runtime.permissions.request()`, and future permission checks will present discrete hosts for approval as being implicitly requested. This value should be saved and restored as needed by the app.

