

- GameKit
-  GKPeerConnectionState Deprecated

Enumeration

# GKPeerConnectionState

The state of a peer known to the session.

macOS 10.8–10.10DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
enum GKPeerConnectionState
```

Deprecated

No longer supported

## Overview

States are not mutually exclusive. For example, a peer can be available for other peers to discover while it is attempting to connect to another peer.

## Topics

### Constants

case stateAvailable

A peer not connected to the session, but one that the session can connect to.

case stateUnavailable

A peer that is no longer interested in receiving connections.

case stateConnected

A peer connected to the session.

case stateDisconnected

A peer that disconnected from the session.

case stateConnecting

A peer attempting to connect to the session.

### Enumeration Cases

case stateConnectedRelay

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

