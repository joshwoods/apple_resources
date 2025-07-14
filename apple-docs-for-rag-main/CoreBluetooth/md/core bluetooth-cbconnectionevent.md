

- Core Bluetooth
-  CBConnectionEvent 

Enumeration

# CBConnectionEvent

A change to the connection state of a peer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
enum CBConnectionEvent
```

## Topics

### Events

case peerConnected

The peer has connected to the local device.

case peerDisconnected

The peer has disconnected from the local device.

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

### Receiving Connection Events

func registerForConnectionEvents(options: [CBConnectionEventMatchingOption : Any]?)

Register for an event notification when the central manager makes a connection matching the given options.

Peripheral Connection Options

Keys used to pass options when connecting to a peripheral.

struct CBConnectionEventMatchingOption

A set of options to use when registering for connection events.

