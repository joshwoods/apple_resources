

- WebKit
- WKWebExtensionContext
-  hasAccess(to:) 

Instance Method

# hasAccess(to:)

Checks the specified URL against the currently granted permission match patterns.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func hasAccess(to url: URL) -> Bool
```

## Parameters 

`url`  

The URL for which to return the status.

## See Also

### Related Documentation

var currentPermissionMatchPatterns: Set&lt;WKWebExtension.MatchPattern>

The currently granted permission match patterns that have not expired.

func hasAccess(to: URL, in: (any WKWebExtensionTab)?) -> Bool

Checks the specified URL against the currently granted permission match patterns in a specific tab.

func permissionStatus(for: URL) -> WKWebExtensionContext.PermissionStatus

Checks the specified URL against the currently denied, granted, and requested permission match patterns.

func permissionStatus(for: URL, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified URL against the currently denied, granted, and requested permission match patterns.

func permissionStatus(for: WKWebExtension.MatchPattern) -> WKWebExtensionContext.PermissionStatus

Checks the specified match pattern against the currently denied, granted, and requested permission match patterns.

func permissionStatus(for: WKWebExtension.MatchPattern, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified match pattern against the currently denied, granted, and requested permission match patterns.

