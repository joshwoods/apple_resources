

- WebKit
- WKWebExtensionContext
-  permissionStatus(for:in:) 

Instance Method

# permissionStatus(for:in:)

Checks the specified URL against the currently denied, granted, and requested permission match patterns.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func permissionStatus(
    for url: URL,
    in tab: (any WKWebExtensionTab)?
) -> WKWebExtensionContext.PermissionStatus
```

## Parameters 

`url`  

The URL for which to return the status.

`tab`  

The tab in which to return the permission status, or `nil` if the tab is not known or the global status is desired.

## Discussion

URLs and match patterns can be granted on a per-tab basis. When the tab is known, access checks should always use this method.

## See Also

### Related Documentation

func permissionStatus(for: URL) -> WKWebExtensionContext.PermissionStatus

Checks the specified URL against the currently denied, granted, and requested permission match patterns.

func hasAccess(to: URL, in: (any WKWebExtensionTab)?) -> Bool

Checks the specified URL against the currently granted permission match patterns in a specific tab.

