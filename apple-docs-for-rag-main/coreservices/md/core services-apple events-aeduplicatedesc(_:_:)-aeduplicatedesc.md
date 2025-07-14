

- Core Services
- Apple Events
-  AEDuplicateDesc(\_:\_:) 

Function

# AEDuplicateDesc(\_:\_:)

Creates a copy of a descriptor.

macOS 10.0+

``` source
func AEDuplicateDesc(
    _ theAEDesc: UnsafePointer!,
    _ result: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAEDesc`  

A pointer to the descriptor to duplicate. See AEDesc.

`result`  

A pointer to a descriptor. On return, the descriptor contains a copy of the descriptor specified by the `theAEDesc` parameter. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of the resulting descriptor after it has finished using it.

## Return Value

A result code. See Result Codes.

## Discussion

It is common for applications to send Apple events that have one or more attributes or parameters in common. For example, if you send a series of Apple events to the same application, the address attribute is the same. In these cases, the most efficient way to create the necessary Apple events is to make a template Apple event that you can then copy—by calling the `AEDuplicateDesc` function—as needed. You then fill in or change the remaining parameters and attributes of the copy, send the copy by calling the `AESend(_:_:_:_:_:_:_:)` function and, after `AESend` returns a result code, dispose of the copy by calling AEDisposeDesc(_:). You can use this approach to prepare structures of type AEDesc, AEDescList, AERecord, and AppleEvent.

### Version-Notes

Thread safe starting in OS X v10.2.

## See Also

### Creating and Duplicating Descriptors

func AECreateDesc(DescType, UnsafeRawPointer!, Size, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a new descriptor that incorporates the specified data.

func AECreateDescFromExternalPtr(OSType, UnsafeRawPointer!, Size, AEDisposeExternalUPP!, SRefCon!, UnsafeMutablePointer&lt;AEDesc>!) -> OSStatus

Creates a new descriptor that uses a memory buffer supplied by the caller.

