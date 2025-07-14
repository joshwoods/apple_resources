

- FSKit
- FSContainerState
-  FSContainerState.notReady 

Case

# FSContainerState.notReady

The container isn’t ready.

macOS 15.4+

``` source
case notReady
```

## See Also

### Container states

case blocked

The container is blocked from transitioning from the not-ready state to the ready state by a potentially-recoverable error.

case ready

The container is ready, but inactive.

case active

The container is active, and one or more volumes are active.

