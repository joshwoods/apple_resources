

- GameKit
-  GKError 

Structure

# GKError

The error structure used by this framework.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct GKError
```

## Mentioned in 

Finding multiple players for a game

## Topics

### Error Codes

enum Code

Error codes for the GameKit error domain.

static var authenticationInProgress: GKError.Code

The system can’t complete the requested operation because the local player is already authenticating.

static var cancelled: GKError.Code

The system canceled the requested operation or the user disabled it.

static var challengeInvalid: GKError.Code

The challenge request failed due to invalid challenge data.

static var communicationsFailure: GKError.Code

The system can’t complete the requested operation due to an error communicating with the server.

static var gameSessionRequestInvalid: GKError.Code

The properties of the game session request are impossible to fulfill.

static var gameUnrecognized: GKError.Code

The system can’t complete the requested operation because Game Center doesn’t recognize the app.

static var invalidCredentials: GKError.Code

The system can’t complete the requested operation because the user name or password are incorrect.

static var invalidParameter: GKError.Code

The system can’t complete the requested operation because one or more parameters are invalid.

static var invalidPlayer: GKError.Code

The system can’t complete the requested operation because the player is invalid.

static var invitationsDisabled: GKError.Code

The system can’t complete the requested operation because the receiving player has disabled invitations.

static var matchNotConnected: GKError.Code

The system can’t complete the requested operation because the match isn’t connected to other players.

static var matchRequestInvalid: GKError.Code

The system can’t complete the requested operation because the match request is invalid.

static var notAuthenticated: GKError.Code

The system can’t complete the requested operation because the system hasn’t authenticated the local player.

static var notSupported: GKError.Code

The app doesn’t have Game Center enabled.

static var parentalControlsBlocked: GKError.Code

The system can’t complete the requested operation because the user disabled this feature in Restrictions.

static var playerPhotoFailure: GKError.Code

The system can’t complete the requested operation to retrieve a player’s photo.

static var playerStatusExceedsMaximumLength: GKError.Code

The player’s status exceeds the maximum length.

static var playerStatusInvalid: GKError.Code

The player’s status is invalid.

static var scoreNotSet: GKError.Code

The system can’t complete the requested operation because the system hasn’t set the score.

static var turnBasedInvalidParticipant: GKError.Code

The system can’t complete the requested operation because the specified participant is invalid.

static var turnBasedInvalidState: GKError.Code

The system can’t complete the requested operation because the session is in an invalid state.

static var turnBasedInvalidTurn: GKError.Code

The system can’t complete the requested operation because the participant doesn’t have the required turn state.

static var turnBasedMatchDataTooLarge: GKError.Code

The system can’t complete the requested operation because the match data is too large.

static var turnBasedTooManySessions: GKError.Code

The system can’t complete the requested operation because it exceeds the maximum number of sessions.

static var ubiquityContainerUnavailable: GKError.Code

The system can’t complete the requested operation because the user hasn’t signed in to iCloud or hasn’t enabled iCloud Drive.

static var underage: GKError.Code

The system can’t complete the requested operation because this feature isn’t available to underage players.

static var unexpectedConnection: GKError.Code

An unexpected player has connected to a match.

static var unknown: GKError.Code

The system can’t complete the requested operation due to an unknown error.

static var userDenied: GKError.Code

The system can’t complete the requested operation because the user denied it.

static var restrictedToAutomatch: GKError.Code

The system can’t complete the requested operation because the player is using automatch.

static var apiNotAvailable: GKError.Code

The system can’t complete the requested operation because the API isn’t available.

static var notAuthorized: GKError.Code

The system can’t complete the requested operation because the system hasn’t authorized the player.

static var connectionTimeout: GKError.Code

The system can’t complete the requested operation because the connection timed out.

static var apiObsolete: GKError.Code

The system can’t complete the requested operation because Apple deprecated the API.

static var iCloudUnavailable: GKError.Code

The system can’t complete the requested operation because it can’t access the player’s iCloud account.

static var lockdownMode: GKError.Code

The system can’t complete the requested operation because the player enabled Lockdown Mode on the device.

static var appUnlisted: GKError.Code

The system can’t complete the requested operation because the game isn’t available on the App Store.

static var friendListDescriptionMissing: GKError.Code

The system denies access to the local player’s friends list because the game didn’t provide a reason.

static var friendListRestricted: GKError.Code

The system restricts access to the local player’s friends list.

static var friendListDenied: GKError.Code

The local player denies access to their friends list.

static var friendRequestNotAvailable: GKError.Code

The player can’t send a friend request at this time from this device.

### Type Properties

static var debugMode: GKError.Code

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Error codes for the GameKit error domain.

let GKErrorDomain: String

The error domain for general game errors.

