

- WebKit
- WKWebExtensionContext
-  permissionStatus(for:) 

Instance Method

# permissionStatus(for:)

Checks the specified match pattern against the currently denied, granted, and requested permission match patterns.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func permissionStatus(for pattern: WKWebExtension.MatchPattern) -> WKWebExtensionContext.PermissionStatus
```

## Parameters 

`pattern`  

The pattern for which to return the status.

## Discussion

Match patterns can be granted on a per-tab basis. When the tab is known, access checks should always use the method that checks in a tab.

## See Also

### Related Documentation

func permissionStatus(for: WKWebExtension.MatchPattern, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified match pattern against the currently denied, granted, and requested permission match patterns.

func hasAccess(to: URL, in: (any WKWebExtensionTab)?) -> Bool

Checks the specified URL against the currently granted permission match patterns in a specific tab.

