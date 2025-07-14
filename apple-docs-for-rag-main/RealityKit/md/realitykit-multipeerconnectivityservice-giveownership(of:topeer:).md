

- RealityKit
- MultipeerConnectivityService
-  giveOwnership(of:toPeer:) 

Instance Method

# giveOwnership(of:toPeer:)

Transfers ownership of the given entity to the named network device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
func giveOwnership(
    of entity: Entity,
    toPeer peer: any SynchronizationPeerID
) -> Bool
```

## Parameters 

`entity`  

The entity whose ownership is transferred.

`peer`  

The networked device receiving ownership.

## Return Value

A Boolean that’s `true` if the ownership transfer succeeds.

## See Also

### Managing ownership

func owner(of: Entity) -> (any SynchronizationPeerID)?

Gets the device that owns a given entity.

