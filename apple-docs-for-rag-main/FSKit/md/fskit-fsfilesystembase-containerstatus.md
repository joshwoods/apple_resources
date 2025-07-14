

- FSKit
- FSFileSystemBase
-  containerStatus 

Instance Property

# containerStatus

The status of the file system container, indicating its readiness and activity.

macOS 15.4+

``` source
@NSCopying
var containerStatus: FSContainerStatus { get set }
```

**Required**

## Discussion

A file system container starts in the FSContainerState.notReady state, and then transitions to the other values of the FSContainerState enumeration. The following diagram illustrates the possible state transitions.

Your file system implementation updates this property as it changes state. Many events and operations may trigger a state transition, and some transitions depend on a specific file system’s design.

When using FSBlockDeviceResource, implement the following common state transitions:

- Calling `loadResource` transitions the state out of FSContainerState.notReady. For all block device file systems, this operation changes the state to either FSContainerState.ready or FSContainerState.blocked.

- Calling `unloadResource` transitions to the FSContainerState.notReady state, as does device termination.

- Transitioning from FSContainerState.blocked to FSContainerState.ready occurs as a result of resolving the underlying block favorably.

- Transitioning from FSContainerState.ready to FSContainerState.blocked is unusal, but valid.

- Transitioning between FSContainerState.ready and FSContainerState.active can result from maintenance operations such as startCheck(task:options:). For a FSUnaryFileSystem, this transition can also occur when activating or deactivating the container’s single volume.

