

- AudioDriverKit
- IOUserAudioBox
-  IsAcquired 

Instance Method

# IsAcquired

Returns a Boolean value that indicates the box’s acquisition state.

DriverKit 21.0+

``` source
bool IsAcquired();
```

## Return Value

`true` if the box is acquired; `false` otherwise.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Managing Acquirability

HandleChangeAcquireBox

Informs the box of a change to its acquisition state.

SetIsAcquired

Set the box’s acquisition state.

SetIsAcquirable

Set the box’s acquirability state.

IsAcquirable

Returns a Boolean value that indicates the box’s acquirabilty state.

SetAcquisitionFailure

Sets the error code to return when box acquisition fails.

GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

