

- StoreKit
- SKCloudServiceAuthorizationStatus
-  SKCloudServiceAuthorizationStatus.restricted Deprecated

Case

# SKCloudServiceAuthorizationStatus.restricted

Access to the music library is restricted in a way that the user cannot change, so your app should not prompt for authorization. An example of this situation is if the device is in an education mode.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
case restricted
```

Deprecated

Use MusicAuthorization.Status from MusicKit

## See Also

### Constants

case notDetermined

The authorization type cannot be determined.

Deprecated

case denied

The user does not authorize any access to their music library.

Deprecated

case authorized

The user authorizes playback of Apple Music tracks and the addition of tracks to their music library.

Deprecated

