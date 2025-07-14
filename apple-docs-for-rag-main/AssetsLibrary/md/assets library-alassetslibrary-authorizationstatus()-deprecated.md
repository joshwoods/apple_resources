

- Assets Library
- ALAssetsLibrary
-  authorizationStatus() Deprecated

Type Method

# authorizationStatus()

Returns photo data authorization status for this application.

iOS 6.0–9.0DeprecatediPadOS 6.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class func authorizationStatus() -> ALAuthorizationStatus
```

Deprecated

Use authorizationStatus on the shared PHPhotoLibrary from the Photos framework instead

## Return Value

Photo data authorization status for this application. For the constants returned, see ALAuthorizationStatus.

## Discussion

This method does not prompt the user for access.

You can use it to detect restricted access and simply hide UI instead of prompting for access.

