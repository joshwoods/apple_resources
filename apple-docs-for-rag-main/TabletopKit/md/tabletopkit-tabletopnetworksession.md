

- TabletopKit
-  TabletopNetworkSession 

Class

# TabletopNetworkSession

An object that coordinates network-related tasks in multiplayer games.

visionOS 2.0+

``` source
class TabletopNetworkSession where Coordinator : TabletopNetworkSessionCoordinator
```

## Overview

To start a multiplayer game for a local player, use the start() method. TabletopKit syncs the current table state between all peers in the session, so update the table state before invoking this method.

After invoking the start() method, the local player becomes the arbiter who ensures that TabletopKit applies actions in order for all players. To switch the arbiter role between players, use the becomeArbiter() and followArbiter(_:) methods.

To join an existing game, use the join() method, and to pass incoming messages to the game, use the processIncomingMessage(_:from:) method.

To get all the people who join the session, not just the players, use the peers property.

## Topics

### Joining multiplayer games

func start()

func join()

func leave()

func terminate()

### Changing the arbiter role between players

func becomeArbiter()

func followArbiter(TabletopNetworkSession&lt;Coordinator>.Peer)

### Managing network session peers

var peers: Set&lt;TabletopNetworkSession&lt;Coordinator>.Peer>

func addPeer(TabletopNetworkSession&lt;Coordinator>.Peer)

func removePeer(TabletopNetworkSession&lt;Coordinator>.Peer)

typealias Peer

### Receiving messages from peers

func processIncomingMessage(Data, from: TabletopNetworkSession&lt;Coordinator>.Peer)

## See Also

### Multiplayer network session

protocol TabletopNetworkSessionCoordinator

A protocol for objects that manage network sessions between peers.

enum TabletopSendMessageResult

The possible results of sending messages in a network session.

