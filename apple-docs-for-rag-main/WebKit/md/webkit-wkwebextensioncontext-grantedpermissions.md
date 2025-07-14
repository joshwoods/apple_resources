

- WebKit
- WKWebExtensionContext
-  grantedPermissions 

Instance Property

# grantedPermissions

The currently granted permissions and their expiration dates.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var grantedPermissions: [WKWebExtension.Permission : Date] { get set }
```

## Discussion

Permissions that don’t expire will have a distant future date. This will never include expired entries at time of access.

Setting this property will replace all existing entries. Use this property for saving and restoring permission status in bulk.

Permissions in this dictionary should be explicitly granted by the user before being added. Any permissions in this collection will not be presented for approval again until they expire. This value should be saved and restored as needed by the app.

## See Also

### Related Documentation

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.Permission)

Sets the status of a permission with a distant future expiration date.

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.Permission, expirationDate: Date?)

Sets the status of a permission with a specific expiration date.

