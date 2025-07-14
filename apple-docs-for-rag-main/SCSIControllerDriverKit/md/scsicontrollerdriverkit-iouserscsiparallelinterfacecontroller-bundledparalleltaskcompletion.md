

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  BundledParallelTaskCompletion 

Instance Method

# BundledParallelTaskCompletion

Indicates to the system that the extension completed a bundled asynchronous request.

DriverKit

``` source
void BundledParallelTaskCompletion(OSAction * action, const uint16_t parallelResponseSlotIndices[32], uint16_t parallelResponseSlotIndicesCount);
```

## Parameters 

`action`  

A pointer to the OSAction object of the asynchronous request that the system specifies in a UserProcessBundledParallelTasks call.

`parallelResponseSlotIndices`  

The indices of the shared response buffer slots containing a SCSIUserParallelResponse for each task to complete.

`parallelResponseSlotIndicesCount`  

The number of tasks to complete. Ensure that entries from zero to `(parallelResponseSlotIndicesCount - 1)` have valid indicies.

## Discussion

Use this method to complete one or more requests previously received by the UserProcessBundledParallelTasks method. For each request to complete:

1.  Populate a SCSIUserParallelResponse.

2.  Make the response available in the shared response buffers.

3.  Pass the response buffer slot in `parallelResponseSlotIndices`.

The command and response buffers have a one-to-one mapping; use the same slot number for related command and response payloads.

## See Also

### Managing Bundled Parallel Tasks

UserProcessBundledParallelTasks

Processes one or more parallel tasks in response to a call from the framework.

UserMapBundledParallelTaskCommandAndResponseBuffers

Maps the shared command and response buffers in the dext address space in response to a call from the framework.

