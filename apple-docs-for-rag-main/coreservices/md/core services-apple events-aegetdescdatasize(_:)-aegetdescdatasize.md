

- Core Services
- Apple Events
-  AEGetDescDataSize(\_:) 

Function

# AEGetDescDataSize(\_:)

Gets the size, in bytes, of the data in the specified descriptor.

macOS 10.0+

``` source
func AEGetDescDataSize(_ theAEDesc: UnsafePointer!) -> Size
```

## Parameters 

`theAEDesc`  

A pointer to the descriptor to obtain the data size for. See AEDesc.

## Return Value

Returns the size, in bytes, of the data in the specified descriptor.

## Discussion

This function works only with value descriptors created by AECreateDesc(_:_:_:_:). You cannot get the data size of an AERecord or AEDescList, for example.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Operating On Descriptor Data

func AEGetDescData(UnsafePointer&lt;AEDesc>!, UnsafeMutableRawPointer!, Size) -> OSErr

Gets the data from the specified descriptor.

func AEGetDescDataRange(UnsafePointer&lt;AEDesc>!, UnsafeMutableRawPointer!, Size, Size) -> OSStatus

Retrieves a specified series of bytes from the specified descriptor.

func AEReplaceDescData(DescType, UnsafeRawPointer!, Size, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Copies the specified data into the specified descriptor, replacing any previous data.

