

- GameKit
- GKError
- GKError.Code
-  GKError.Code.underage 

Case

# GKError.Code.underage

The system can’t complete the requested operation because this feature isn’t available to underage players.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
case underage
```

## See Also

### Player-Related Errors

case userDenied

The system can’t complete the requested operation because the user denied it.

case invalidCredentials

The system can’t complete the requested operation because the user name or password are incorrect.

case notAuthenticated

The system can’t complete the requested operation because the system hasn’t authorized the player.

case authenticationInProgress

The system can’t complete the requested operation because the local player is already authenticating.

case parentalControlsBlocked

The system can’t complete the requested operation because the user disabled this feature in Restrictions.

case playerStatusExceedsMaximumLength

The player’s status exceeds the maximum length.

case playerStatusInvalid

The player’s status is invalid.

case playerPhotoFailure

The system can’t complete the requested operation to retrieve a player’s photo.

case ubiquityContainerUnavailable

The system can’t complete the requested operation because the user hasn’t signed in to iCloud or hasn’t enabled iCloud Drive.

case notAuthorized

The system can’t complete the requested operation because the system hasn’t authorized the player.

case iCloudUnavailable

The system can’t complete the requested operation because it can’t access the player’s iCloud account.

case lockdownMode

The system can’t complete the requested operation because the player enabled Lockdown Mode on the device.

