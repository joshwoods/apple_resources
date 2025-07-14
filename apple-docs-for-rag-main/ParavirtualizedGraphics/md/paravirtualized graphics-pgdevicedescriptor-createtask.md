

- Paravirtualized Graphics
- PGDeviceDescriptor
-  createTask 

Instance Property

# createTask

A handler that the framework calls to create a task object.

Mac Catalyst 14.0+macOS 11.0+

``` source
var createTask: PGCreateTask? { get set }
```

## See Also

### Managing Tasks

var destroyTask: PGDestroyTask?

A handler that the framework calls to destroy a task object.

typealias PGCreateTask

The block signature for a routine that creates a task.

typealias PGDestroyTask

The block signature for a routine that destroys a task.

