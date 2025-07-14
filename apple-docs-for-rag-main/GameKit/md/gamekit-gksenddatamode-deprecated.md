

- GameKit
-  GKSendDataMode Deprecated

Enumeration

# GKSendDataMode

The mechanism used to transmit data to other peers.

macOS 10.8–10.10DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
enum GKSendDataMode
```

Deprecated

No longer supported

## Topics

### Constants

case reliable

The data is sent continuously until it is successfully received by the intended recipients or the connection times out.

case unreliable

The data is sent once and is not sent again if a transmission error occurred.

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

