

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserAbortTaskSetRequest 

Instance Method

# UserAbortTaskSetRequest

Aborts all tasks in a logical unit.

DriverKit

``` source
kern_return_t UserAbortTaskSetRequest(uint64_t theT, uint64_t theL, uint32_t * response);
```

## Parameters 

`theT`  

The target containing the tasks to abort.

`theL`  

The logical unit containing the tasks to abort.

`response`  

On return, a SCSI protocol-specific value indicating the success or failure of the request.

## Discussion

This method doesn’t clear previously established conditions, such as `MODE SELECT` parameters, reservations, and autocontingent allegiance (ACA) attributes.

## See Also

### Performing SCSI Standard Task Management

UserAbortTaskRequest

Aborts a single task.

UserClearACARequest

Removes an autocontingent allegiance (ACA) attribute from a logical unit’s task set.

UserClearTaskSetRequest

Aborts all tasks in a logical unit and clears their data.

UserLogicalUnitResetRequest

Resets a logical unit.

UserTargetResetRequest

Resets a target.

