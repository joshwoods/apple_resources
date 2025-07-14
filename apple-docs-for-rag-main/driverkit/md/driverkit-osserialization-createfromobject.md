

- DriverKit
- OSSerialization
-  createFromObject 

Static Method

# createFromObject

Allocates an OSSerialization object with the serialized data of an object.

DriverKitiOSiPadOSmacOS

``` source
static OSSerializationPtr createFromObject(OSObjectPtr const object);
```

## Parameters 

`object`  

Object to serialize. Only certain DriverKit classes may be serialized: OSData, OSString, OSNumber, OSBoolean, OSArray, OSDictionary.

## Return Value

NULL on failure, otherwise the allocated OSSerialization with reference count 1 to be released by the caller.

## Discussion

Allocates an OSSerialization object with the serialized data of an object.

## See Also

### Creating a Serialization Object

createFromBytes

Allocates an OSSerialization object from the serialized data of a previous serialization.

OSCreateSerializationFromBytes

OSCreateSerializationFromObject

free

OSSerializationFreeBufferHandler

OSSerializationPtr

