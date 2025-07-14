

- AVFoundation
- AVAuthorizationStatus
-  AVAuthorizationStatus.notDetermined 

Case

# AVAuthorizationStatus.notDetermined

A status that indicates the user hasn’t yet granted or denied authorization.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.14+tvOS 17.0+visionOS 1.0+

``` source
case notDetermined
```

## Mentioned in 

Requesting authorization to capture and save media

## Discussion

This is the default status prior to user to granting or denying recording priviledge to the app. Call requestAccess(for:completionHandler:) to prompt the user for permission.

## See Also

### Status Values

case restricted

A status that indicates the app isn’t permitted to use media capture devices.

case denied

A status that indicates the user has explicitly denied an app permission to capture media.

case authorized

A status that indicates the user has explicitly granted an app permission to capture media.

