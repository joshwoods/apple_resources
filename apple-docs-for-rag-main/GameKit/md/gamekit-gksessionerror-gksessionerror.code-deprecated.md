

- GameKit
- GKSessionError
-  GKSessionError.Code Deprecated

Enumeration

# GKSessionError.Code

Error codes for the session error domain.

tvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
enum Code
```

Deprecated

No longer supported

## Topics

### Constants

case invalidParameterError

A parameter had an unexpected value.

case peerNotFoundError

A peer with the specified `peerID` string could not be found.

case declinedError

The peer your application tried to connect to refused the connection.

case timedOutError

The operation could not be completed in the specified timeout period.

case cancelledError

A peer that invited the session to connect to them canceled the connection request.

case connectionFailedError

The attempt to establish a connection with another peer failed.

case connectionClosedError

The connection to another peer closed unexpectedly.

case dataTooBigError

The data your application attempted to send was too large for the session to transmit in a single call.

case notConnectedError

Reserved for future use.

case cannotEnableError

Bluetooth is not currently available.

case inProgressError

The peer your application attempted to connect to has already requested a connection to your session.

case connectivityError

An error occurred in the GKSession object’s connection code.

case transportError

An error occurred in the GKSession object’s transport code.

case internalError

A serious error occurred inside GKSession.

case unknownError

Reserved for when the error does not fit in another category above.

case systemError

An error occurred outside of the GKSession object’s control, such as memory allocation.

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

struct GKSessionErrorDeprecated

enum GKSessionMode

Modes that determine how a session interacts with other peers.

Deprecated

enum Code

Error codes for the voice chat service error domain.

Deprecated

struct GKVoiceChatServiceErrorDeprecated

