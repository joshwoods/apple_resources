

- DriverKit
- OSSerialization
-  finalizeBuffer 

Instance Method

# finalizeBuffer

Obtain the result of the serialization performed by createFromObject().

DriverKitiOSiPadOSmacOS

``` source
const void * finalizeBuffer(size_t * length);
```

## Parameters 

`length`  

The length of the serialization data.

## Return Value

NULL on failure, otherwise a pointer to the serialization data. It is valid only while the OSSerialization object is retained.

## Discussion

Obtain the result of the serialization performed by createFromObject().

## See Also

### Getting the Serialized Content

copyObject

Obtain the result of the deserialization performed by createFromBytes().

OSCreateObjectFromSerialization

OSSerializationGetBytes

