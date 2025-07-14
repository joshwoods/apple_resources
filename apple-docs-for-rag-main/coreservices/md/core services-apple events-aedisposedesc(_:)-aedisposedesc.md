

- Core Services
- Apple Events
-  AEDisposeDesc(\_:) 

Function

# AEDisposeDesc(\_:)

Deallocates the memory used by a descriptor.

macOS 10.0+

``` source
func AEDisposeDesc(_ theAEDesc: UnsafeMutablePointer!) -> OSErr
```

## Parameters 

`theAEDesc`  

A pointer to the descriptor to deallocate. On return, a null descriptor. If you pass a null descriptor in this parameter, `AEDisposeDesc` returns `noErr`. See AEDesc.

## Return Value

A result code. See Result Codes. As currently implemented, `AEDisposeDesc` always returns `noErr`.

## Discussion

The `AEDisposeDesc` function deallocates the memory used by a descriptor. After calling this method, the descriptor becomes an empty descriptor with a type of `typeNULL`. Because all Apple event structures (except for keyword-specified descriptors) are descriptors, you can use `AEDisposeDesc` for any of them.

Do not call `AEDisposeDesc` on a descriptor obtained from another Apple Event Manager function (such as the reply event from a call to `AESend(_:_:_:_:_:_:_:)`) unless that function returns successfully.

### Special Considerations

If the `AEDesc` might contain an OSL token, dispose of it with AEDisposeToken(_:).

### Version-Notes

Thread safe starting in OS X v10.2.

