

- FSKit
- FSContainerState
-  FSContainerState.active 

Case

# FSContainerState.active

The container is active, and one or more volumes are active.

macOS 15.4+

``` source
case active
```

## See Also

### Container states

case notReady

The container isn’t ready.

case blocked

The container is blocked from transitioning from the not-ready state to the ready state by a potentially-recoverable error.

case ready

The container is ready, but inactive.

