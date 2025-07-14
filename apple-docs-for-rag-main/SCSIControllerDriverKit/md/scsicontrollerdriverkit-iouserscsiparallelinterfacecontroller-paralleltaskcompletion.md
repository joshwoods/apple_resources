

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  ParallelTaskCompletion 

Instance Method

# ParallelTaskCompletion

Indicates to the system that the extension has completed an asynchronous request.

DriverKit

``` source
void ParallelTaskCompletion(OSAction * action, SCSIUserParallelResponse response);
```

## Parameters 

`action`  

A pointer to the OSAction object of the asynchronous request that the system specifies in a UserProcessParallelTask.

`response`  

The result of the asychronous request.

## Discussion

Your driver extension class invokes this method to complete an asynchronous request.

## See Also

### Managing Tasks

UserProcessParallelTask

Processes a parallel task in response to a call from the framework.

SCSIUserParallelTask

The properties of a parallel task to perform.

SCSIUserParallelResponse

The properties of a completed request.

