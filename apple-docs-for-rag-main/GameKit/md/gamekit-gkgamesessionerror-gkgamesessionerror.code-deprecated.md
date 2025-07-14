

- GameKit
- GKGameSessionError
-  GKGameSessionError.Code Deprecated

Enumeration

# GKGameSessionError.Code

Error codes for the game session domain.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum Code
```

Deprecated

Use the real-time and turn-based matchmaking APIs instead.

## Topics

### Enumeration Cases

case unknown

The requested operation could not be completed due to an unknown error.

case notAuthenticated

The requested operation could not be completed because you are not signed in to iCloud.

case sessionConflict

The requested operation could not be completed because the session has been updated on the server, causing a conflict.

case sessionNotShared

The requested operation could not be completed because this session has not been shared with other players.

case connectionCancelledByUser

The requested operation could not be completed because the connection to the session was cancelled.

case connectionFailed

The requested operation could not be completed because the session could not find other players to connect to.

case sessionHasMaxConnectedPlayers

The requested operation could not be completed because the session has reached the maximum number of connected players.

case sendDataNotConnected

The requested operation could not be completed because you are not connected to the session.

case sendDataNoRecipients

The requested operation could not be completed because there are no recipients connected to session.

case sendDataNotReachable

The requested operation could not be completed because one or more players is not reachable.

case sendRateLimitReached

The requested operation could not be completed because you have reached the limits for save data request.

case badContainer

The requested operation could not be completed because the iCloud container is invalid.

case cloudQuotaExceeded

The requested operation could not be completed because the user’s iCloud quota would be exceeded.

case networkFailure

The requested operation could not be completed due to an error communicating with the server.

case cloudDriveDisabled

The requested operation could not be completed because iCloud Drive has been disabled for the application.

case invalidSession

The requested operation could not be completed because the Game Session does not exist or the player is not part of the game session.

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

### Deprecated enumerations

enum GKPeerConnectionState

The state of a peer known to the session.

Deprecated

enum GKPeerPickerConnectionType

Network connections available to the peer picker dialog.

Deprecated

enum GKSendDataMode

The mechanism used to transmit data to other peers.

Deprecated

enum Code

Error codes for the session error domain.

Deprecated

struct GKSessionErrorDeprecated

enum GKSessionMode

Modes that determine how a session interacts with other peers.

Deprecated

enum Code

Error codes for the voice chat service error domain.

Deprecated

struct GKVoiceChatServiceErrorDeprecated

