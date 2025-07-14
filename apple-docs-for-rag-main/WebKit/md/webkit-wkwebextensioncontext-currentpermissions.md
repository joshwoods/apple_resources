

- WebKit
- WKWebExtensionContext
-  currentPermissions 

Instance Property

# currentPermissions

The currently granted permissions that have not expired.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var currentPermissions: Set { get }
```

## See Also

### Related Documentation

var grantedPermissions: [WKWebExtension.Permission : Date]

The currently granted permissions and their expiration dates.

