

- Core Services
- Apple Events
-  AERemoveCoercionHandler(\_:\_:\_:\_:) 

Function

# AERemoveCoercionHandler(\_:\_:\_:\_:)

Removes a coercion handler from a coercion handler dispatch table.

macOS 10.0+

``` source
func AERemoveCoercionHandler(
    _ fromType: DescType,
    _ toType: DescType,
    _ handler: AECoercionHandlerUPP!,
    _ isSysHandler: Bool
) -> OSErr
```

## Parameters 

`fromType`  

The descriptor type of the data coerced by the handler. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`toType`  

The descriptor type of the resulting data. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`handler`  

A universal procedure pointer to the coercion handler to remove. Although the parameters `fromType` and `toType` are sufficient to identify the handler, you can identify the handler explicitly as a safeguard. If you pass `NULL` for this parameter, the Apple Event Manager relies solely on the event class and event ID to identify the handler. See AECoercionHandlerUPP.

`isSysHandler`  

Specifies the coercion table to remove the handler from. Pass `TRUE` to remove the handler from the system coercion table or `FALSE` to remove the handler from your application’s coercion table. Use of the system coercion table is not recommended.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

Use of system coercion tables is not recommended. For more information, see Writing and Installing Coercion Handlers in Apple Events Programming Guide.

## See Also

### Managing Coercion Handler Dispatch Tables

func AEGetCoercionHandler(DescType, DescType, UnsafeMutablePointer&lt;AECoercionHandlerUPP?>!, UnsafeMutablePointer&lt;SRefCon?>!, UnsafeMutablePointer&lt;DarwinBoolean>!, Bool) -> OSErr

Gets the coercion handler for a specified descriptor type.

func AEInstallCoercionHandler(DescType, DescType, AECoercionHandlerUPP!, SRefCon!, Bool, Bool) -> OSErr

Installs a coercion handler in either the application or system coercion handler dispatch table.

