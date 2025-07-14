

- WebKit
- WKWebExtensionContext
-  setPermissionStatus(\_:for:) 

Instance Method

# setPermissionStatus(\_:for:)

Sets the permission status of a URL with a distant future expiration date.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func setPermissionStatus(
    _ status: WKWebExtensionContext.PermissionStatus,
    for url: URL
)
```

## Parameters 

`status`  

The new permission status to set for the given URL.

`url`  

The URL for which to set the status.

## Discussion

The URL is converted into a match pattern and will update grantedPermissionMatchPatterns and deniedPermissionMatchPatterns. Use this method for changing a single URL’s status. Only WKWebExtensionContext.PermissionStatus.deniedExplicitly, WKWebExtensionContext.PermissionStatus.unknown, and WKWebExtensionContext.PermissionStatus.grantedExplicitly states are allowed to be set using this method.

## See Also

### Related Documentation

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: URL, expirationDate: Date?)

Sets the permission status of a URL with a distant future expiration date.

