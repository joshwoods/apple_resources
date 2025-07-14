

- StoreKit
-  SKCloudServiceAuthorizationStatus Deprecated

Enumeration

# SKCloudServiceAuthorizationStatus

Constants that indicate the type of authorization the customer has for accessing the Music library.

iOS 9.3–18.0DeprecatediPadOS 9.3–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 9.3–18.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
enum SKCloudServiceAuthorizationStatus
```

Deprecated

Use MusicAuthorization.Status from MusicKit

## Topics

### Constants

case notDetermined

The authorization type cannot be determined.

case denied

The user does not authorize any access to their music library.

case restricted

Access to the music library is restricted in a way that the user cannot change, so your app should not prompt for authorization. An example of this situation is if the device is in an education mode.

case authorized

The user authorizes playback of Apple Music tracks and the addition of tracks to their music library.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting authorization to access the Music library

Requesting Access to Apple Music Library

Prompt the customer to authorize access to Apple Music library.

class func authorizationStatus() -> SKCloudServiceAuthorizationStatus

Returns the type of authorization the customer has for accessing the Music library on the device.

Deprecated

class func requestAuthorization((SKCloudServiceAuthorizationStatus) -> Void)

Asks the customer for permission to access the Music library on the device.

Deprecated

