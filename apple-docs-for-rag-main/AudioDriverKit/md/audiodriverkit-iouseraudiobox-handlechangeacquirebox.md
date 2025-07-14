

- AudioDriverKit
- IOUserAudioBox
-  HandleChangeAcquireBox 

Instance Method

# HandleChangeAcquireBox

Informs the box of a change to its acquisition state.

DriverKit 21.0+

``` source
kern_return_t HandleChangeAcquireBox(bool in_acquire);
```

## Parameters 

`in_acquire`  

A Boolean value that indicates the acquisition state. If this value is `true`, the box is being acquired.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation calls SetIsAcquired and return kIOReturnSuccess. Custom drivers should override this method to validate the change, then return kIOReturnSuccess to confirm the change. If acquisition fails, return the error code returned from GetAcquisitionFailure.

## See Also

### Managing Acquirability

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

GetAcquisitionFailure

Returns the error code for use when box acquisition fails.

