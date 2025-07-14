

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserClearACARequest 

Instance Method

# UserClearACARequest

Removes an autocontingent allegiance (ACA) attribute from a logical unit’s task set.

DriverKit

``` source
kern_return_t UserClearACARequest(uint64_t theT, uint64_t theL, uint32_t * response);
```

## Parameters 

`theT`  

The target containing the tasks to clear ACA attributes from.

`theL`  

The logical unit containing the tasks to clear ACA attributes from.

`response`  

On return, a SCSI protocol-specific value indicating the success or failure of the request.

## See Also

### Performing SCSI Standard Task Management

UserAbortTaskRequest

Aborts a single task.

UserAbortTaskSetRequest

Aborts all tasks in a logical unit.

UserClearTaskSetRequest

Aborts all tasks in a logical unit and clears their data.

UserLogicalUnitResetRequest

Resets a logical unit.

UserTargetResetRequest

Resets a target.

