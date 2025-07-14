

- Paravirtualized Graphics
- PGDeviceDescriptor
-  destroyTask 

Instance Property

# destroyTask

A handler that the framework calls to destroy a task object.

Mac Catalyst 14.0+macOS 11.0+

``` source
var destroyTask: PGDestroyTask? { get set }
```

## See Also

### Managing Tasks

var createTask: PGCreateTask?

A handler that the framework calls to create a task object.

typealias PGCreateTask

The block signature for a routine that creates a task.

typealias PGDestroyTask

The block signature for a routine that destroys a task.

