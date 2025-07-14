

- RealityKit
- SynchronizationComponent
- SynchronizationComponent.OwnershipTransferCompletionResult
-  SynchronizationComponent.OwnershipTransferCompletionResult.timedOut 

Case

# SynchronizationComponent.OwnershipTransferCompletionResult.timedOut

The ownership transfer request timed out.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
case timedOut
```

## Discussion

A timeout doesn’t necessarily mean that the request is denied. It might succeed after the timeout.

## See Also

### Ownership transfer completion results

case granted

The request is accepted and ownership is transferred.

