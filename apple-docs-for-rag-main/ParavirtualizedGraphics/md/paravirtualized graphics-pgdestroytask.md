

- Paravirtualized Graphics
-  PGDestroyTask 

Type Alias

# PGDestroyTask

The block signature for a routine that destroys a task.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGDestroyTask = (OpaquePointer) -> Void
```

## Parameters 

`task`  

The task to destroy.

## Discussion

The block must clean up any virtual memory that the device object allocated when it created the task.

## See Also

### Managing Tasks

var createTask: PGCreateTask?

A handler that the framework calls to create a task object.

var destroyTask: PGDestroyTask?

A handler that the framework calls to destroy a task object.

typealias PGCreateTask

The block signature for a routine that creates a task.

