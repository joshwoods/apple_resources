

- FSKit
- FSContainerState
-  FSContainerState.ready 

Case

# FSContainerState.ready

The container is ready, but inactive.

macOS 15.4+

``` source
case ready
```

## See Also

### Container states

case notReady

The container isn’t ready.

case blocked

The container is blocked from transitioning from the not-ready state to the ready state by a potentially-recoverable error.

case active

The container is active, and one or more volumes are active.

