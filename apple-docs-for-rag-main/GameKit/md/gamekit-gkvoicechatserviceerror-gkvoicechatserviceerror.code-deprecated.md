

- GameKit
- GKVoiceChatServiceError
-  GKVoiceChatServiceError.Code Deprecated

Enumeration

# GKVoiceChatServiceError.Code

Error codes for the voice chat service error domain.

tvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
enum Code
```

Deprecated

No longer supported

## Topics

### Constants

case internalError

A serious error occurred inside the voice chat service.

case noRemotePacketsError

The voice chat service stopped receiving packets from the remote participant.

case unableToConnectError

The voice chat service was unable to establish a connection with another user.

case remoteParticipantHangupError

The remote participant in a voice chat stopped the chat.

case invalidCallIDError

The voice chat service didn’t recognize the call identifier.

case audioUnavailableError

The audio hardware is unavailable to the voice chat service.

case uninitializedClientError

The application did not set a client before calling voice chat service methods.

case clientMissingRequiredMethodsError

The voice chat service did not find an expected method defined by the client.

case remoteParticipantBusyError

The remote participant is already connected to a voice chat.

case remoteParticipantCancelledError

A remote participant attempted to start a voice chat, then canceled.

case remoteParticipantResponseInvalidError

Invalid data was received from a remote participant.

case remoteParticipantDeclinedInviteError

A remote participant declined an invitation.

case methodCurrentlyInvalidError

A method on the voice chat service was called when it was not allowed to be called (for example, attempting to connect when the voice chat service was already connected).

case networkConfigurationError

The voice chat service had problems accessing the network.

case unsupportedRemoteVersionError

The other participant is running a different version of the voice chat service.

case outOfMemoryError

The voice chat service was unable to allocate memory required to operate.

case invalidParameterError

A parameter had an unrecognized value.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated enumerations

enum Code

Error codes for the game session domain.

Deprecated

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

struct GKVoiceChatServiceErrorDeprecated

