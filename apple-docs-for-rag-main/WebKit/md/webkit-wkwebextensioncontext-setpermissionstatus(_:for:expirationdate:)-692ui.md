

- WebKit
- WKWebExtensionContext
-  setPermissionStatus(\_:for:expirationDate:) 

Instance Method

# setPermissionStatus(\_:for:expirationDate:)

Sets the status of a permission with a specific expiration date.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func setPermissionStatus(
    _ status: WKWebExtensionContext.PermissionStatus,
    for permission: WKWebExtension.Permission,
    expirationDate: Date?
)
```

## Parameters 

`status`  

The new permission status to set for the given permission.

`permission`  

The permission for which to set the status.

`expirationDate`  

The expiration date for the new permission status, or \c nil for distant future.

## Discussion

This method will update grantedPermissions and deniedPermissions. Use this method for changing a single permission’s status.

Passing a `nil` expiration date will be treated as a distant future date. Only WKWebExtensionContext.PermissionStatus.deniedExplicitly, WKWebExtensionContext.PermissionStatus.unknown, and WKWebExtensionContext.PermissionStatus.grantedExplicitly states are allowed to be set using this method.

## See Also

### Related Documentation

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.Permission)

Sets the status of a permission with a distant future expiration date.

