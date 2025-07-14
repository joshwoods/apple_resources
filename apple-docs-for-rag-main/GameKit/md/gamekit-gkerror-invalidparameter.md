

- GameKit
- GKError
-  invalidParameter 

Type Property

# invalidParameter

The system can’t complete the requested operation because one or more parameters are invalid.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
static var invalidParameter: GKError.Code { get }
```

## Discussion

For example, this error code may be returned if your application attempts to post a score and provides a category string that does not match a category you configured for your leaderboards in App Store Connect.

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

