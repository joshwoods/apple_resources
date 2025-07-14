

- Core Services
- Apple Events
-  AESizeOfFlattenedDesc(\_:) 

Function

# AESizeOfFlattenedDesc(\_:)

Returns the amount of buffer space needed to store the descriptor after flattening it.

macOS 10.0+

``` source
func AESizeOfFlattenedDesc(_ theAEDesc: UnsafePointer!) -> Size
```

## Parameters 

`theAEDesc`  

A pointer to the descriptor to be flattened. See AEDesc.

## Return Value

The size, in bytes, required to store the flattened descriptor.

## Discussion

You call this function before calling AEFlattenDesc(_:_:_:_:) to determine the required size of the buffer for the flatten operation.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Serializing Apple Event Data

func AEFlattenDesc(UnsafePointer&lt;AEDesc>!, Ptr!, Size, UnsafeMutablePointer&lt;Size>!) -> OSStatus

Flattens the specified descriptor and stores the data in the supplied buffer.

func AEUnflattenDesc(UnsafeRawPointer!, UnsafeMutablePointer&lt;AEDesc>!) -> OSStatus

Unflattens the data in the passed buffer and creates a descriptor from it.

Deprecated

