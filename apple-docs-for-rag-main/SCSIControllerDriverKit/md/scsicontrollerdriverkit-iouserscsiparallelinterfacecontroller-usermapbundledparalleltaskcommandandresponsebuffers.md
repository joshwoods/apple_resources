

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserMapBundledParallelTaskCommandAndResponseBuffers 

Instance Method

# UserMapBundledParallelTaskCommandAndResponseBuffers

Maps the shared command and response buffers in the dext address space in response to a call from the framework.

DriverKit

``` source
kern_return_t UserMapBundledParallelTaskCommandAndResponseBuffers(IOBufferMemoryDescriptor * parallelCommandIOMemoryDescriptor, IOBufferMemoryDescriptor * parallelResponseIOMemoryDescriptor);
```

## Parameters 

`parallelCommandIOMemoryDescriptor`  

The memory descriptor corresponding to the command buffers.

`parallelResponseIOMemoryDescriptor`  

The memory descriptor corresponding to the response buffers.

## Return Value

kIOReturnSuccess on success and kIOReturnError on failure.

## Discussion

To optimize the interaction with the DriverKit Extension (dext) class, SCSIControllerDriverKit allocates contiguous command and response buffers to hold the maximum number of tasks reported by UserReportMaximumTaskCount. The framework calls this method before UserStartController, so the dext class can map these buffers in the dext address space. The framework uses the shared buffers to pass command and response payloads. The command and response buffers use a one-to-one mapping; use the same slot number for related command and response payloads. For example, if the framework assigns buffer slot number 12 to a command, use slot number 12 in the mapped response buffers during I/O completion.

The framework owns the shared buffer slots for both command and responses until it passes ownership to the dext in the UserProcessBundledParallelTasks call. From that point, the dext has ownership of these buffer slots until it returns ownership back to the framework in BundledParallelTaskCompletion. Don’t access a command or response buffer slot until the framework passes ownership to your dext.

If you don’t want to use the shared buffers, your dext can return kIOReturnError and continue to use UserProcessParallelTask and `UserCompleteParallelTask` to process the I/O. If you return kIOReturnSuccess from this method, the framework expects your dext to use UserProcessBundledParallelTasks and `UserCompleteBundledParallelTask`.

## See Also

### Managing Bundled Parallel Tasks

UserProcessBundledParallelTasks

Processes one or more parallel tasks in response to a call from the framework.

BundledParallelTaskCompletion

Indicates to the system that the extension completed a bundled asynchronous request.

