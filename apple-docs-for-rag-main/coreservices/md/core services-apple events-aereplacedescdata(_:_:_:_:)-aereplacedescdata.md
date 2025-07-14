

- Core Services
- Apple Events
-  AEReplaceDescData(\_:\_:\_:\_:) 

Function

# AEReplaceDescData(\_:\_:\_:\_:)

Copies the specified data into the specified descriptor, replacing any previous data.

macOS 10.0+

``` source
func AEReplaceDescData(
    _ typeCode: DescType,
    _ dataPtr: UnsafeRawPointer!,
    _ dataSize: Size,
    _ theAEDesc: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`typeCode`  

Specifies the descriptor type of the data pointed to by `dataPtr`. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataPtr`  

A pointer to the data to store in the specified descriptor.

`dataSize`  

The size, in bytes, of the data pointed to by the `dataSize` parameter.

`theAEDesc`  

A pointer to a descriptor. On return, contains the copied data. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

## See Also

### Operating On Descriptor Data

func AEGetDescData(UnsafePointer&lt;AEDesc>!, UnsafeMutableRawPointer!, Size) -> OSErr

Gets the data from the specified descriptor.

func AEGetDescDataSize(UnsafePointer&lt;AEDesc>!) -> Size

Gets the size, in bytes, of the data in the specified descriptor.

func AEGetDescDataRange(UnsafePointer&lt;AEDesc>!, UnsafeMutableRawPointer!, Size, Size) -> OSStatus

Retrieves a specified series of bytes from the specified descriptor.

