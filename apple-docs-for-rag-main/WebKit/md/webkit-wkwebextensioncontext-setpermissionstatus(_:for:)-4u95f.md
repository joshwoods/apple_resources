

- WebKit
- WKWebExtensionContext
-  setPermissionStatus(\_:for:) 

Instance Method

# setPermissionStatus(\_:for:)

Sets the status of a permission with a distant future expiration date.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func setPermissionStatus(
    _ status: WKWebExtensionContext.PermissionStatus,
    for permission: WKWebExtension.Permission
)
```

## Parameters 

`status`  

The new permission status to set for the given permission.

`permission`  

The permission for which to set the status.

## Discussion

This method will update grantedPermissions and deniedPermissions. Use this method for changing a single permission’s status.

Only WKWebExtensionContext.PermissionStatus.deniedExplicitly, WKWebExtensionContext.PermissionStatus.unknown, and WKWebExtensionContext.PermissionStatus.grantedExplicitly states are allowed to be set using this method.

## See Also

### Related Documentation

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.Permission, expirationDate: Date?)

Sets the status of a permission with a specific expiration date.

