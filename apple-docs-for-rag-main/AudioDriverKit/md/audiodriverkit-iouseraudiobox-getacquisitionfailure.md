

- AudioDriverKit
- IOUserAudioBox
-  GetAcquisitionFailure 

Instance Method

# GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

DriverKit 21.0+

``` source
kern_return_t GetAcquisitionFailure();
```

## Return Value

An error code for use when box acquisition fails.

## Discussion

Call this method to retrieve the error to return from a failed call to HandleChangeAcquireBox.

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

SetAcquisitionFailure

Sets the error code to return when box acquisition fails.

