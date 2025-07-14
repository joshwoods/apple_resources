

- Core Services
- Apple Events
-  AEGetDescData(\_:\_:\_:) 

Function

# AEGetDescData(\_:\_:\_:)

Gets the data from the specified descriptor.

macOS 10.0+

``` source
func AEGetDescData(
    _ theAEDesc: UnsafePointer!,
    _ dataPtr: UnsafeMutableRawPointer!,
    _ maximumSize: Size
) -> OSErr
```

## Parameters 

`theAEDesc`  

A pointer to the descriptor to get the data from. See AEDesc.

`dataPtr`  

A pointer to a buffer, local variable, or other storage location created and disposed of by your application. The size in bytes should be the same as the value you pass in the `maximumSize` parameter. On return, contains the data from the descriptor.

`maximumSize`  

The length, in bytes, of the expected descriptor data. The `AEGetDescData` function will not return more data than you specify in this parameter. You typically determine the maximum size by calling AEGetDescDataSize(_:).

## Return Value

A result code. See Result Codes.

## Discussion

Your application can call AEGetDescDataSize(_:) to get the size, in bytes, of the data in a descriptor, allocate a buffer or variable of that size, then call `AEGetDescData` to get the data.

This function works only with value descriptors created by AECreateDesc(_:_:_:_:). You cannot get the data of an AERecord or AEDescList, for example.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Operating On Descriptor Data

func AEGetDescDataSize(UnsafePointer&lt;AEDesc>!) -> Size

Gets the size, in bytes, of the data in the specified descriptor.

func AEGetDescDataRange(UnsafePointer&lt;AEDesc>!, UnsafeMutableRawPointer!, Size, Size) -> OSStatus

Retrieves a specified series of bytes from the specified descriptor.

func AEReplaceDescData(DescType, UnsafeRawPointer!, Size, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Copies the specified data into the specified descriptor, replacing any previous data.

