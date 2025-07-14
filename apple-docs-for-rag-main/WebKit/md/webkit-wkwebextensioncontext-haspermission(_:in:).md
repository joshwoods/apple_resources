

- WebKit
- WKWebExtensionContext
-  hasPermission(\_:in:) 

Instance Method

# hasPermission(\_:in:)

Checks the specified permission against the currently granted permissions in a specific tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func hasPermission(
    _ permission: WKWebExtension.Permission,
    in tab: (any WKWebExtensionTab)?
) -> Bool
```

## Parameters 

`permission`  

The permission for which to return the status.

`tab`  

The tab in which to return the permission status, or `nil` if the tab is not known or the global status is desired.

## Discussion

Permissions can be granted on a per-tab basis. When the tab is known, permission checks should always use this method.

## See Also

### Related Documentation

var currentPermissions: Set&lt;WKWebExtension.Permission>

The currently granted permissions that have not expired.

func hasPermission(WKWebExtension.Permission) -> Bool

Checks the specified permission against the currently granted permissions.

func permissionStatus(for: WKWebExtension.Permission) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

func permissionStatus(for: WKWebExtension.Permission, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

