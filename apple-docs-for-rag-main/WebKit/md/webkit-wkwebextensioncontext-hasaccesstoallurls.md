

- WebKit
- WKWebExtensionContext
-  hasAccessToAllURLs 

Instance Property

# hasAccessToAllURLs

A Boolean value indicating if the currently granted permission match patterns set contains the `` pattern.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasAccessToAllURLs: Bool { get }
```

## Discussion

This does not check for any `*` host patterns. In most cases you should use the broader hasAccessToAllHosts.

## See Also

### Related Documentation

var currentPermissionMatchPatterns: Set&lt;WKWebExtension.MatchPattern>

The currently granted permission match patterns that have not expired.

var hasAccessToAllHosts: Bool

A Boolean value indicating if the currently granted permission match patterns set contains the `` pattern or any `*` host patterns.

