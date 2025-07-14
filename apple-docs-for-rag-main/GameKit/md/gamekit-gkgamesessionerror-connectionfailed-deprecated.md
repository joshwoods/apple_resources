

- GameKit
- GKGameSessionError
-  connectionFailed Deprecated

Type Property

# connectionFailed

The requested operation could not be completed because the session could not find other players to connect to.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static var connectionFailed: GKGameSessionError.Code { get }
```

Deprecated

GKGameSession is deprecated, use real-time and turn-based matchmaking APIs instead.

## See Also

### Error Codes

static var badContainer: GKGameSessionError.Code

The requested operation could not be completed because the iCloud container is invalid.

Deprecated

static var cloudDriveDisabled: GKGameSessionError.Code

The requested operation could not be completed because iCloud Drive has been disabled for the application.

Deprecated

static var cloudQuotaExceeded: GKGameSessionError.Code

The requested operation could not be completed because the user’s iCloud quota would be exceeded.

Deprecated

static var connectionCancelledByUser: GKGameSessionError.Code

The requested operation could not be completed because the connection to the session was cancelled.

Deprecated

static var invalidSession: GKGameSessionError.Code

The requested operation could not be completed because the Game Session does not exist or the player is not part of the game session.

Deprecated

static var networkFailure: GKGameSessionError.Code

The requested operation could not be completed due to an error communicating with the server.

Deprecated

static var notAuthenticated: GKGameSessionError.Code

The requested operation could not be completed because you are not signed in to iCloud.

Deprecated

static var sendDataNoRecipients: GKGameSessionError.Code

The requested operation could not be completed because there are no recipients connected to session.

Deprecated

static var sendDataNotConnected: GKGameSessionError.Code

The requested operation could not be completed because you are not connected to the session.

Deprecated

static var sendDataNotReachable: GKGameSessionError.Code

The requested operation could not be completed because one or more players is not reachable.

Deprecated

static var sendRateLimitReached: GKGameSessionError.Code

The requested operation could not be completed because you have reached the limits for save data request.

Deprecated

static var sessionConflict: GKGameSessionError.Code

The requested operation could not be completed because the session has been updated on the server, causing a conflict.

Deprecated

static var sessionHasMaxConnectedPlayers: GKGameSessionError.Code

The requested operation could not be completed because the session has reached the maximum number of connected players.

Deprecated

static var sessionNotShared: GKGameSessionError.Code

The requested operation could not be completed because this session has not been shared with other players.

Deprecated

static var unknown: GKGameSessionError.Code

The requested operation could not be completed due to an unknown error.

Deprecated

