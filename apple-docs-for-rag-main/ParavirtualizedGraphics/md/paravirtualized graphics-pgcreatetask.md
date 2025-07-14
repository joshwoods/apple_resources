

- Paravirtualized Graphics
-  PGCreateTask 

Type Alias

# PGCreateTask

The block signature for a routine that creates a task.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGCreateTask = (UInt64, UnsafeMutablePointer) -> OpaquePointer?
```

## Parameters 

`vmSize`  

The size of the virtual memory reservation to make for this task.

`baseAddress`  

On return, the block writes the base-host virtually contiguous address for this task.

## Return Value

A PGTask_t pointer, or `NULL` if an error occurred.

## Discussion

The paravirtualization framework calls this block to request memory for a task. The block allocates virtual memory for the task and returns it to the framework. The block also records any data it needs to keep track of this task and returns a pointer to that data. The framework uses this pointer to identify the task in other operations. The framework never accesses the contents of the PGTask_t pointer.

## See Also

### Managing Tasks

var createTask: PGCreateTask?

A handler that the framework calls to create a task object.

var destroyTask: PGDestroyTask?

A handler that the framework calls to destroy a task object.

typealias PGDestroyTask

The block signature for a routine that destroys a task.

