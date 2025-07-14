

- AVFoundation
- AVAuthorizationStatus
-  AVAuthorizationStatus.restricted 

Case

# AVAuthorizationStatus.restricted

A status that indicates the app isn’t permitted to use media capture devices.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.14+tvOS 17.0+visionOS 1.0+

``` source
case restricted
```

## Discussion

This status occurs when a user can’t change the authorization status, possibly due to the system imposing restrictions like parental controls.

## See Also

### Status Values

case notDetermined

A status that indicates the user hasn’t yet granted or denied authorization.

case denied

A status that indicates the user has explicitly denied an app permission to capture media.

case authorized

A status that indicates the user has explicitly granted an app permission to capture media.

