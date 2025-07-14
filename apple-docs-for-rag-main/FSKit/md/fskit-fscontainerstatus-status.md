

- FSKit
- FSContainerStatus
-  status 

Instance Property

# status

An optional error that provides further information about the state.

macOS 15.4+

``` source
var status: (any Error)? { get }
```

## See Also

### Inspecting status properties

var state: FSContainerState

A value that represents the container state, such as ready, active, or blocked.

enum FSContainerState

An enumeration of container state values.

