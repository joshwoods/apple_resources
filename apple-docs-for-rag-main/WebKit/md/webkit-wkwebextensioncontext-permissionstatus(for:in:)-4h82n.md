

- WebKit
- WKWebExtensionContext
-  permissionStatus(for:in:) 

Instance Method

# permissionStatus(for:in:)

Checks the specified permission against the currently denied, granted, and requested permissions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func permissionStatus(
    for permission: WKWebExtension.Permission,
    in tab: (any WKWebExtensionTab)?
) -> WKWebExtensionContext.PermissionStatus
```

## Parameters 

`permission`  

The permission for which to return the status.

`tab`  

The tab in which to return the permission status, or `nil` if the tab is not known or the global status is desired.

## Discussion

Permissions can be granted on a per-tab basis. When the tab is known, access checks should always specify the tab.

## See Also

### Related Documentation

func permissionStatus(for: WKWebExtension.Permission) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

func hasPermission(WKWebExtension.Permission, in: (any WKWebExtensionTab)?) -> Bool

Checks the specified permission against the currently granted permissions in a specific tab.

