

- AudioDriverKit
- IOUserAudioBox
-  SetAcquisitionFailure 

Instance Method

# SetAcquisitionFailure

Sets the error code to return when box acquisition fails.

DriverKit 21.0+

``` source
kern_return_t SetAcquisitionFailure(kern_return_t in_failure_code);
```

## Parameters 

`in_failure_code`  

An error code to return when box acquisition fails.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Set this code to provide the error to return from failed calls to HandleChangeAcquireBox.

If successful, changing the acquisition failure code sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Managing Acquirability

HandleChangeAcquireBox

Informs the box of a change to its acquisition state.

SetIsAcquired

Set the box’s acquisition state.

IsAcquired

Returns a Boolean value that indicates the box’s acquisition state.

SetIsAcquirable

Set the box’s acquirability state.

IsAcquirable

Returns a Boolean value that indicates the box’s acquirabilty state.

GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

