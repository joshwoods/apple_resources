

- RealityKit
- SynchronizationComponent
- SynchronizationComponent.OwnershipTransferMode
-  SynchronizationComponent.OwnershipTransferMode.manual 

Case

# SynchronizationComponent.OwnershipTransferMode.manual

Require explicit ownership request confirmation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
case manual
```

## Discussion

Handle the SynchronizationEvents.OwnershipRequest event to find out when a peer requests ownership of an entity, and call the method stored in the requests’s accept property to confirm the transfer of ownership.

## See Also

### Ownership transfer modes

case autoAccept

Grant ownership requests automatically.

