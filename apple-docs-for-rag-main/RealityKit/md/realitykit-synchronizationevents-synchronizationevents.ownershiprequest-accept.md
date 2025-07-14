

- RealityKit
- SynchronizationEvents
- SynchronizationEvents.OwnershipRequest
-  accept 

Instance Property

# accept

The callback function that the current owner calls to grant ownership to the requesting peer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
let accept: () -> Void
```

## Discussion

If an entity’s ownershipTransferMode property is set to SynchronizationComponent.OwnershipTransferMode.autoAccept, the entity automatically grants ownership to any other entity that requests it.

In case you configure an entity to have a transfer mode of SynchronizationComponent.OwnershipTransferMode.manual, then when you receive an SynchronizationEvents.OwnershipRequest event, call the accept method to complete the transfer of ownership.

