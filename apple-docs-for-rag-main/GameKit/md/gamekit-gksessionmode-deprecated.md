

- GameKit
-  GKSessionMode Deprecated

Enumeration

# GKSessionMode

Modes that determine how a session interacts with other peers.

macOS 10.8–10.10DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
enum GKSessionMode
```

Deprecated

No longer supported

## Topics

### Constants

case server

A server advertises itself to local devices using its sessionID property.

case client

A client searches for servers advertising the same sessionID property.

case peer

A peer advertises like a server and searches like a client.

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

enum Code

Error codes for the voice chat service error domain.

Deprecated

struct GKVoiceChatServiceErrorDeprecated

