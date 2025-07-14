

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserClearTaskSetRequest 

Instance Method

# UserClearTaskSetRequest

Aborts all tasks in a logical unit and clears their data.

DriverKit

``` source
kern_return_t UserClearTaskSetRequest(uint64_t theT, uint64_t theL, uint32_t * response);
```

## Parameters 

`theT`  

The target containing the tasks to clear.

`theL`  

The logical unit containing the tasks to clear.

`response`  

On return, a SCSI protocol-specific value indicating the success or failure of the request.

## Discussion

This method clears all pending and status data, but not previously established conditions, such as `MODE SELECT` parameters, reservations, and autocontingent allegiance (ACA) attributes.

## See Also

### Performing SCSI Standard Task Management

UserAbortTaskRequest

Aborts a single task.

UserAbortTaskSetRequest

Aborts all tasks in a logical unit.

UserClearACARequest

Removes an autocontingent allegiance (ACA) attribute from a logical unit’s task set.

UserLogicalUnitResetRequest

Resets a logical unit.

UserTargetResetRequest

Resets a target.

