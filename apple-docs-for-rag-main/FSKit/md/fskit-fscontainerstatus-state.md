

- FSKit
- FSContainerStatus
-  state 

Instance Property

# state

A value that represents the container state, such as ready, active, or blocked.

macOS 15.4+

``` source
var state: FSContainerState { get }
```

## See Also

### Inspecting status properties

enum FSContainerState

An enumeration of container state values.

var status: (any Error)?

An optional error that provides further information about the state.

