

- RealityKit
- SynchronizationComponent
-  ownershipTransferMode 

Instance Property

# ownershipTransferMode

The entity’s transfer ownership mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var ownershipTransferMode: SynchronizationComponent.OwnershipTransferMode
```

## Discussion

By default, the transfer mode is SynchronizationComponent.OwnershipTransferMode.autoAccept. You can set it to SynchronizationComponent.OwnershipTransferMode.manual to require explicit confirmation of the request by your app.

## See Also

### Managing ownership

var isOwner: Bool

A Boolean that indicates whether the calling process owns the entity.

