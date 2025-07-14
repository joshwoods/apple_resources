

- AudioDriverKit
- IOUserAudioObject
-  GetName 

Instance Method

# GetName

Gets the name of the object.

DriverKit 21.0+

``` source
OSSharedPtr GetName();
```

## Return Value

A `OSSharedPtr` to an OSString containing the object name.

## Discussion

Getting the name synchronizes by using the work queue created by the object.

## See Also

### Working with Object Names

SetName

Sets the name of the object.

