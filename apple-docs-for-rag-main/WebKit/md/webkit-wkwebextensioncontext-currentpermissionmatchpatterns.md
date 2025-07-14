

- WebKit
- WKWebExtensionContext
-  currentPermissionMatchPatterns 

Instance Property

# currentPermissionMatchPatterns

The currently granted permission match patterns that have not expired.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var currentPermissionMatchPatterns: Set { get }
```

## See Also

### Related Documentation

var grantedPermissionMatchPatterns: [WKWebExtension.MatchPattern : Date]

The currently granted permission match patterns and their expiration dates.

