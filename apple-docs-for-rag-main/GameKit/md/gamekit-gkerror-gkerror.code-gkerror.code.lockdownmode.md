

- GameKit
- GKError
- GKError.Code
-  GKError.Code.lockdownMode 

Case

# GKError.Code.lockdownMode

The system can’t complete the requested operation because the player enabled Lockdown Mode on the device.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
case lockdownMode
```

## Discussion

For more information about Lockdown Mode, see About Lockdown Mode.

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

case underage

The system can’t complete the requested operation because this feature isn’t available to underage players.

case playerPhotoFailure

The system can’t complete the requested operation to retrieve a player’s photo.

case ubiquityContainerUnavailable

The system can’t complete the requested operation because the user hasn’t signed in to iCloud or hasn’t enabled iCloud Drive.

case notAuthorized

The system can’t complete the requested operation because the system hasn’t authorized the player.

case iCloudUnavailable

The system can’t complete the requested operation because it can’t access the player’s iCloud account.

