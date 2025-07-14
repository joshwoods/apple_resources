

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserTargetResetRequest 

Instance Method

# UserTargetResetRequest

Resets a target.

DriverKit

``` source
kern_return_t UserTargetResetRequest(uint64_t theT, uint32_t * response);
```

## Parameters 

`theT`  

The target to reset.

`response`  

On return, a SCSI protocol-specific value indicating the success or failure of the request.

## Discussion

The definition of the reset event that this request performs depends on the SCSI protocol.

## See Also

### Performing SCSI Standard Task Management

UserAbortTaskRequest

Aborts a single task.

UserAbortTaskSetRequest

Aborts all tasks in a logical unit.

UserClearACARequest

Removes an autocontingent allegiance (ACA) attribute from a logical unit’s task set.

UserClearTaskSetRequest

Aborts all tasks in a logical unit and clears their data.

UserLogicalUnitResetRequest

Resets a logical unit.

