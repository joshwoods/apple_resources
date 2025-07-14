

- AudioDriverKit
- IOUserAudioBox
-  IsAcquirable 

Instance Method

# IsAcquirable

Returns a Boolean value that indicates the box’s acquirabilty state.

DriverKit 21.0+

``` source
bool IsAcquirable();
```

## Return Value

`true` if the box is acquirable; `false` otherwise.

## Discussion

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

SetAcquisitionFailure

Sets the error code to return when box acquisition fails.

GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

