

- Core Services
- Apple Events
-  AECreateDesc(\_:\_:\_:\_:) 

Function

# AECreateDesc(\_:\_:\_:\_:)

Creates a new descriptor that incorporates the specified data.

macOS 10.0+

``` source
func AECreateDesc(
    _ typeCode: DescType,
    _ dataPtr: UnsafeRawPointer!,
    _ dataSize: Size,
    _ result: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`typeCode`  

The descriptor type for the new descriptor. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`dataPtr`  

A pointer to the data for the new descriptor. This data is copied into a newly-allocated block of memory for the descriptor that is created. To minimize copying overhead, consider using AECreateDescFromExternalPtr(_:_:_:_:_:_:).

`dataSize`  

The length, in bytes, of the data for the new descriptor.

`result`  

A pointer to a descriptor. On successful return, a descriptor that incorporates the data specified by the `dataPtr` parameter. On error, a null descriptor. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of the resulting descriptor after it has finished using it. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

While it is possible to create an Apple event descriptor or a descriptor list or a descriptor with the `AECreateDesc` function (assuming you have access to the raw data for an Apple event, list, or descriptor), you typically create these structured objects with their specific creation routines—`AECreateAppleEvent`, `AECreateList`, or `AECreateDesc`.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Creating and Duplicating Descriptors

func AECreateDescFromExternalPtr(OSType, UnsafeRawPointer!, Size, AEDisposeExternalUPP!, SRefCon!, UnsafeMutablePointer&lt;AEDesc>!) -> OSStatus

Creates a new descriptor that uses a memory buffer supplied by the caller.

func AEDuplicateDesc(UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a copy of a descriptor.

