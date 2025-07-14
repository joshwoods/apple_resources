

- FSKit
- FSContainerState
-  FSContainerState.blocked 

Case

# FSContainerState.blocked

The container is blocked from transitioning from the not-ready state to the ready state by a potentially-recoverable error.

macOS 15.4+

``` source
case blocked
```

## Discussion

This state implies that the error has a resolution that would allow the container to become ready, such as correcting an incorrect password.

## See Also

### Container states

case notReady

The container isn’t ready.

case ready

The container is ready, but inactive.

case active

The container is active, and one or more volumes are active.

