

- GameKit
-  GKGameSessionError Deprecated

Structure

# GKGameSessionError

Error codes for the game session domain.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
struct GKGameSessionError
```

Deprecated

GKGameSession is deprecated, use real-time and turn-based matchmaking APIs instead.

## Topics

### Error Codes

static var badContainer: GKGameSessionError.Code

The requested operation could not be completed because the iCloud container is invalid.

static var cloudDriveDisabled: GKGameSessionError.Code

The requested operation could not be completed because iCloud Drive has been disabled for the application.

static var cloudQuotaExceeded: GKGameSessionError.Code

The requested operation could not be completed because the user’s iCloud quota would be exceeded.

static var connectionCancelledByUser: GKGameSessionError.Code

The requested operation could not be completed because the connection to the session was cancelled.

static var connectionFailed: GKGameSessionError.Code

The requested operation could not be completed because the session could not find other players to connect to.

static var invalidSession: GKGameSessionError.Code

The requested operation could not be completed because the Game Session does not exist or the player is not part of the game session.

static var networkFailure: GKGameSessionError.Code

The requested operation could not be completed due to an error communicating with the server.

static var notAuthenticated: GKGameSessionError.Code

The requested operation could not be completed because you are not signed in to iCloud.

static var sendDataNoRecipients: GKGameSessionError.Code

The requested operation could not be completed because there are no recipients connected to session.

static var sendDataNotConnected: GKGameSessionError.Code

The requested operation could not be completed because you are not connected to the session.

static var sendDataNotReachable: GKGameSessionError.Code

The requested operation could not be completed because one or more players is not reachable.

static var sendRateLimitReached: GKGameSessionError.Code

The requested operation could not be completed because you have reached the limits for save data request.

static var sessionConflict: GKGameSessionError.Code

The requested operation could not be completed because the session has been updated on the server, causing a conflict.

static var sessionHasMaxConnectedPlayers: GKGameSessionError.Code

The requested operation could not be completed because the session has reached the maximum number of connected players.

static var sessionNotShared: GKGameSessionError.Code

The requested operation could not be completed because this session has not been shared with other players.

static var unknown: GKGameSessionError.Code

The requested operation could not be completed due to an unknown error.

enum Code

Error codes for the game session domain.

### Error Domain

let GKGameSessionErrorDomain: String

The error domain for game sessions.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Deprecated structures

struct GKVoiceChatServiceErrorDeprecated

struct GKSessionErrorDeprecated

