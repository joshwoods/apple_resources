

- AudioDriverKit
- IOUserAudioBox
-  SetIsProtected 

Instance Method

# SetIsProtected

Sets a Boolean value that indicates if the box requires authentication before use.

DriverKit 21.0+

``` source
kern_return_t SetIsProtected(bool in_is_protected);
```

## Parameters 

`in_is_protected`  

The new value of the box’s protection state.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the protection state sends a notification to the host to update the object state.

This method synchronizes by using the work queue created by the object.

## See Also

### Managing Protection State

IsProtected

Returns a Boolean value that indicates if the box requires authentication before use.

