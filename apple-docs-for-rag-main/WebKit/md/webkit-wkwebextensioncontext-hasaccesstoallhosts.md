

- WebKit
- WKWebExtensionContext
-  hasAccessToAllHosts 

Instance Property

# hasAccessToAllHosts

A Boolean value indicating if the currently granted permission match patterns set contains the `` pattern or any `*` host patterns.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasAccessToAllHosts: Bool { get }
```

## See Also

### Related Documentation

var currentPermissionMatchPatterns: Set&lt;WKWebExtension.MatchPattern>

The currently granted permission match patterns that have not expired.

var hasAccessToAllURLs: Bool

A Boolean value indicating if the currently granted permission match patterns set contains the `` pattern.

