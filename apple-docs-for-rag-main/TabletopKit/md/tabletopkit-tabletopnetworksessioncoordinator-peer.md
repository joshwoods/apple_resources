

- TabletopKit
- TabletopNetworkSessionCoordinator
-  Peer 

Associated Type

# Peer

visionOS 2.0+

``` source
associatedtype Peer : Hashable, Identifiable where Self.Peer.ID == UUID
```

**Required**

## See Also

### Managing network session peers

func peerJoinedGame(Self.Peer.ID)

**Required**

func peerLeftGame(Self.Peer.ID)

**Required**

