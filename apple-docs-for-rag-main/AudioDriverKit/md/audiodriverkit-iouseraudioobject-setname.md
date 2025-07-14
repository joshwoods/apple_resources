

- AudioDriverKit
- IOUserAudioObject
-  SetName 

Instance Method

# SetName

Sets the name of the object.

DriverKit 21.0+

``` source
kern_return_t SetName(OSString * in_name);
```

## Parameters 

`in_name`  

The name to set, as an OSString.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If the change succeeds, the framework sends a notification to the host to update its object state. Setting the name synchronizes by using the work queue created by the object.

## See Also

### Working with Object Names

GetName

Gets the name of the object.

