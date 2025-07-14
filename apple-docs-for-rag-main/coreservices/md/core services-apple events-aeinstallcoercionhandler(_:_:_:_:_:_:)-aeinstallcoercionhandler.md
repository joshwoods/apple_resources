

- Core Services
- Apple Events
-  AEInstallCoercionHandler(\_:\_:\_:\_:\_:\_:) 

Function

# AEInstallCoercionHandler(\_:\_:\_:\_:\_:\_:)

Installs a coercion handler in either the application or system coercion handler dispatch table.

macOS 10.0+

``` source
func AEInstallCoercionHandler(
    _ fromType: DescType,
    _ toType: DescType,
    _ handler: AECoercionHandlerUPP!,
    _ handlerRefcon: SRefCon!,
    _ fromTypeIsDesc: Bool,
    _ isSysHandler: Bool
) -> OSErr
```

## Parameters 

`fromType`  

The descriptor type of the data coerced by the handler. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`toType`  

The descriptor type of the resulting data. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants.

If there was already an entry in the specified coercion handler table for the same source descriptor type and result descriptor type, the existing entry is replaced. See DescType.

`handler`  

A universal procedure pointer to the coercion handler function to install. See AECoercionHandlerUPP.

`handlerRefcon`  

A reference constant. The Apple Event Manager passes this value to the handler each time it calls it. If your handler doesn’t require a reference constant, pass 0 for this parameter.

`fromTypeIsDesc`  

Specifies the form of the data to coerce. Pass `TRUE` if the coercion handler expects the data as a descriptor or `FALSE` if the coercion handler expects a pointer to the data. The Apple Event Manager can provide a pointer to data more efficiently than it can provide a descriptor, so all coercion functions should accept a pointer to data if possible.

`isSysHandler`  

Specifies the coercion table to add the handler to. Pass `TRUE` to add the handler to the system coercion table or `FALSE` to add the handler to your application’s coercion table. Use of the system coercion table is not recommended.

## Return Value

A result code. See Result Codes.

## Discussion

Before using `AEInstallCoercionHandler` to install a handler for a particular descriptor type, you can use the AEGetCoercionHandler(_:_:_:_:_:_:) function to determine whether the table already contains a coercion handler for that type.

### Version-Notes

See the Version Notes section for the AECoercePtr(_:_:_:_:_:) function for information on when to use descriptor-based versus pointer-based coercion handlers starting in OS X version 10.2.

Thread safe starting in OS X v10.2.

Your application should not install a coercion handler in a system coercion handler dispatch table with the goal that the handler will get called when other applications perform coercions—this won’t work in macOS. For more information, see Writing and Installing Coercion Handlers in Apple Events Programming Guide.

## See Also

### Managing Coercion Handler Dispatch Tables

func AEGetCoercionHandler(DescType, DescType, UnsafeMutablePointer&lt;AECoercionHandlerUPP?>!, UnsafeMutablePointer&lt;SRefCon?>!, UnsafeMutablePointer&lt;DarwinBoolean>!, Bool) -> OSErr

Gets the coercion handler for a specified descriptor type.

func AERemoveCoercionHandler(DescType, DescType, AECoercionHandlerUPP!, Bool) -> OSErr

Removes a coercion handler from a coercion handler dispatch table.

