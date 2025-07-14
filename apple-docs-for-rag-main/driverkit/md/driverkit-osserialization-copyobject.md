

- DriverKit
- OSSerialization
-  copyObject 

Instance Method

# copyObject

Obtain the result of the deserialization performed by createFromBytes().

DriverKitiOSiPadOSmacOS

``` source
OSObjectPtr copyObject();
```

## Return Value

NULL on failure, otherwise the allocated OSObject with reference count 1 to be released by the caller.

## Discussion

Obtain the result of the deserialization performed by createFromBytes().

## See Also

### Getting the Serialized Content

OSCreateObjectFromSerialization

OSSerializationGetBytes

finalizeBuffer

Obtain the result of the serialization performed by createFromObject().

