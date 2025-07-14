

- TabletopKit
-  TabletopNetworkSessionCoordinator 

Protocol

# TabletopNetworkSessionCoordinator

A protocol for objects that manage network sessions between peers.

visionOS 2.0+

``` source
protocol TabletopNetworkSessionCoordinator
```

## Overview

Peers are networking participants that might or might not join a multiplayer game.

## Topics

### Starting network sessions

func coordinateWithSession(Self.NetworkSession)

**Required**

typealias NetworkSession

### Managing network session peers

func peerJoinedGame(Self.Peer.ID)

**Required**

func peerLeftGame(Self.Peer.ID)

**Required**

associatedtype Peer : Hashable, Identifiable

**Required**

### Sending messages between peers

func sendMessage(Data, to: Set&lt;Self.Peer>, completion: (TabletopSendMessageResult) -> Void)

**Required**

func sendMessageUnreliably(Data, to: Set&lt;Self.Peer>, completion: (TabletopSendMessageResult) -> Void)

**Required**

## See Also

### Multiplayer network session

class TabletopNetworkSession

An object that coordinates network-related tasks in multiplayer games.

enum TabletopSendMessageResult

The possible results of sending messages in a network session.

