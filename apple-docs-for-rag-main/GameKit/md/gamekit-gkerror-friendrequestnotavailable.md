

- GameKit
- GKError
-  friendRequestNotAvailable 

Type Property

# friendRequestNotAvailable

The player can’t send a friend request at this time from this device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var friendRequestNotAvailable: GKError.Code { get }
```

## See Also

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

