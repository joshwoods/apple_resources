

- AudioDriverKit
- IOUserAudioBox
-  SetIsAcquired 

Instance Method

# SetIsAcquired

Set the box’s acquisition state.

DriverKit 21.0+

``` source
kern_return_t SetIsAcquired(bool in_is_acquired);
```

## Parameters 

`in_is_acquired`  

The new value of the box’s acquisition state.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the acquisition state sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Managing Acquirability

HandleChangeAcquireBox

Informs the box of a change to its acquisition state.

IsAcquired

Returns a Boolean value that indicates the box’s acquisition state.

SetIsAcquirable

Set the box’s acquirability state.

IsAcquirable

Returns a Boolean value that indicates the box’s acquirabilty state.

SetAcquisitionFailure

Sets the error code to return when box acquisition fails.

GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

