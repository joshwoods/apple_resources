

- FSKit
-  FSContainerState 

Enumeration

# FSContainerState

An enumeration of container state values.

macOS 15.4+

``` source
enum FSContainerState
```

## Overview

This enumeration represents values for a container’s state engine. Containers start in the FSContainerState.notReady state.

## Topics

### Container states

case notReady

The container isn’t ready.

case blocked

The container is blocked from transitioning from the not-ready state to the ready state by a potentially-recoverable error.

case ready

The container is ready, but inactive.

case active

The container is active, and one or more volumes are active.

### Working with raw values

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting status properties

var state: FSContainerState

A value that represents the container state, such as ready, active, or blocked.

var status: (any Error)?

An optional error that provides further information about the state.

