

- AudioDriverKit
- IOUserAudioDriver
-  PropertiesChanged 

Instance Method

# PropertiesChanged

Informs the host when the state of an object in the driver changes.

DriverKit 21.0+

``` source
kern_return_t PropertiesChanged(IOUserAudioObjectID in_object_id, IOUserAudioObjectPropertySelector * in_properties, uint32_t in_num_properties);
```

## Parameters 

`in_object_id`  

The identifier of the object whose properties changed.

`in_properties`  

An array of IOUserAudioObjectPropertySelector instances for the changed properties.

`in_num_properties`  

The number of elements in the `in_properties` array.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

For device objects, only use this method for state changes that don’t affect IO or the structure of the device.

## See Also

### Communicating with the Host

IOUserAudioObjectPropertySelector

A four character code which, along with the scope and element, specific piece of information about an audio object.

