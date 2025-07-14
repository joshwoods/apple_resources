

- WebKit
- WKWebExtensionContext
-  hasPermission(\_:) 

Instance Method

# hasPermission(\_:)

Checks the specified permission against the currently granted permissions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func hasPermission(_ permission: WKWebExtension.Permission) -> Bool
```

## Parameters 

`permission`  

The permission for which to return the status.

## See Also

### Related Documentation

var currentPermissions: Set&lt;WKWebExtension.Permission>

The currently granted permissions that have not expired.

func hasPermission(WKWebExtension.Permission, in: (any WKWebExtensionTab)?) -> Bool

Checks the specified permission against the currently granted permissions in a specific tab.

func permissionStatus(for: WKWebExtension.Permission) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

func permissionStatus(for: WKWebExtension.Permission, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

