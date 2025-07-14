

- RealityKit
- MultipeerConnectivityService
-  owner(of:) 

Instance Method

# owner(of:)

Gets the device that owns a given entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
func owner(of entity: Entity) -> (any SynchronizationPeerID)?
```

## Parameters 

`entity`  

The entity for which you want the owner.

## Return Value

The networked device that owns the entity.

## See Also

### Managing ownership

func giveOwnership(of: Entity, toPeer: any SynchronizationPeerID) -> Bool

Transfers ownership of the given entity to the named network device.

