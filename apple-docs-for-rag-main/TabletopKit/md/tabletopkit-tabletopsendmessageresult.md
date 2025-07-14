

- TabletopKit
-  TabletopSendMessageResult 

Enumeration

# TabletopSendMessageResult

The possible results of sending messages in a network session.

visionOS 2.0+

``` source
enum TabletopSendMessageResult
```

## Topics

### Message results

case success

Message was sent successfully

case failure

Message sending failed, and network condition is effectively disconnected

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Multiplayer network session

class TabletopNetworkSession

An object that coordinates network-related tasks in multiplayer games.

protocol TabletopNetworkSessionCoordinator

A protocol for objects that manage network sessions between peers.

