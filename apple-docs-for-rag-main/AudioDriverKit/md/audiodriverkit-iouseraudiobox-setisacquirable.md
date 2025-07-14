

- AudioDriverKit
- IOUserAudioBox
-  SetIsAcquirable 

Instance Method

# SetIsAcquirable

Set the box’s acquirability state.

DriverKit 21.0+

``` source
kern_return_t SetIsAcquirable(bool in_is_acquirable);
```

## Parameters 

`in_is_acquirable`  

The new value of the box’s acquirability state.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the acquirability state sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Managing Acquirability

HandleChangeAcquireBox

Informs the box of a change to its acquisition state.

SetIsAcquired

Set the box’s acquisition state.

IsAcquired

Returns a Boolean value that indicates the box’s acquisition state.

IsAcquirable

Returns a Boolean value that indicates the box’s acquirabilty state.

SetAcquisitionFailure

Sets the error code to return when box acquisition fails.

GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

