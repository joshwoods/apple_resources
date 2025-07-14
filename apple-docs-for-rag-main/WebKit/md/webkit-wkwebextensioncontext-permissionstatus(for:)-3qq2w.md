

- WebKit
- WKWebExtensionContext
-  permissionStatus(for:) 

Instance Method

# permissionStatus(for:)

Checks the specified permission against the currently denied, granted, and requested permissions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func permissionStatus(for permission: WKWebExtension.Permission) -> WKWebExtensionContext.PermissionStatus
```

## Parameters 

`permission`  

The permission for which to return the status.

## Discussion

Permissions can be granted on a per-tab basis. When the tab is known, access checks should always use the method that checks in a tab.

## See Also

### Related Documentation

func permissionStatus(for: WKWebExtension.Permission, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

func hasPermission(WKWebExtension.Permission) -> Bool

Checks the specified permission against the currently granted permissions.

