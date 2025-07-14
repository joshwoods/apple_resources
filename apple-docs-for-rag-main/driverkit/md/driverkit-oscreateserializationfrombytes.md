

- DriverKit
-  OSCreateSerializationFromBytes 

Function

# OSCreateSerializationFromBytes

DriverKitiOSiPadOSmacOS

``` source
OSSerializationPtr OSCreateSerializationFromBytes(const void * bytes, size_t length, OSSerializationFreeBufferHandlerfreeBuffer);
```

## See Also

### Creating a Serialization Object

createFromBytes

Allocates an OSSerialization object from the serialized data of a previous serialization.

createFromObject

Allocates an OSSerialization object with the serialized data of an object.

OSCreateSerializationFromObject

free

OSSerializationFreeBufferHandler

OSSerializationPtr

