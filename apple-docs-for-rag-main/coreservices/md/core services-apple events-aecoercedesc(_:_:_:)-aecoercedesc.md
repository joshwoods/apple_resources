

- Core Services
- Apple Events
-  AECoerceDesc(\_:\_:\_:) 

Function

# AECoerceDesc(\_:\_:\_:)

Coerces the data in a descriptor to another descriptor type and creates a descriptor containing the newly coerced data.

macOS 10.0+

``` source
func AECoerceDesc(
    _ theAEDesc: UnsafePointer!,
    _ toType: DescType,
    _ result: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`theAEDesc`  

A pointer to the descriptor containing the data to coerce. See AEDesc.

`toType`  

The desired descriptor type of the resulting descriptor. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`result`  

A pointer to a descriptor. On successful return, a descriptor containing the coerced data and matching the descriptor type specified in `toType`. On error, a null descriptor. If the function returns successfully, your application should call the AEDisposeDesc(_:) function to dispose of the resulting descriptor after it has finished using it.

## Return Value

A result code. See Result Codes. If `AECoerceDesc` returns a nonzero result code, it returns a null descriptor record (a descriptor record of type `typeNull`, which does not contain any data) unless the Apple Event Manager is not available because of limited memory.

## Discussion

See the Version Notes section for the AECoercePtr(_:_:_:_:_:) function for information on when to use descriptor-based versus pointer-based coercion handlers starting in OS X version 10.2.

Thread safe starting in OS X v10.2.

## See Also

### Coercing Descriptor Types

func AECoercePtr(DescType, UnsafeRawPointer!, Size, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Coerces data to a desired descriptor type and creates a descriptor containing the newly coerced data.

