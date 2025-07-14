

- GameKit
- GKGameSessionError
- GKGameSessionError.Code
-  GKGameSessionError.Code.networkFailure Deprecated

Case

# GKGameSessionError.Code.networkFailure

The requested operation could not be completed due to an error communicating with the server.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
case networkFailure
```

Deprecated

GKGameSession is deprecated, use real-time and turn-based matchmaking APIs instead.

## See Also

### Enumeration Cases

case unknown

The requested operation could not be completed due to an unknown error.

Deprecated

case notAuthenticated

The requested operation could not be completed because you are not signed in to iCloud.

Deprecated

case sessionConflict

The requested operation could not be completed because the session has been updated on the server, causing a conflict.

Deprecated

case sessionNotShared

The requested operation could not be completed because this session has not been shared with other players.

Deprecated

case connectionCancelledByUser

The requested operation could not be completed because the connection to the session was cancelled.

Deprecated

case connectionFailed

The requested operation could not be completed because the session could not find other players to connect to.

Deprecated

case sessionHasMaxConnectedPlayers

The requested operation could not be completed because the session has reached the maximum number of connected players.

Deprecated

case sendDataNotConnected

The requested operation could not be completed because you are not connected to the session.

Deprecated

case sendDataNoRecipients

The requested operation could not be completed because there are no recipients connected to session.

Deprecated

case sendDataNotReachable

The requested operation could not be completed because one or more players is not reachable.

Deprecated

case sendRateLimitReached

The requested operation could not be completed because you have reached the limits for save data request.

Deprecated

case badContainer

The requested operation could not be completed because the iCloud container is invalid.

Deprecated

case cloudQuotaExceeded

The requested operation could not be completed because the user’s iCloud quota would be exceeded.

Deprecated

case cloudDriveDisabled

The requested operation could not be completed because iCloud Drive has been disabled for the application.

Deprecated

case invalidSession

The requested operation could not be completed because the Game Session does not exist or the player is not part of the game session.

Deprecated

