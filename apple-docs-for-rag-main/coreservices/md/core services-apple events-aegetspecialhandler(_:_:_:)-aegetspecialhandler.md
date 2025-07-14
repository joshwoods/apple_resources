

- Core Services
- Apple Events
-  AEGetSpecialHandler(\_:\_:\_:) 

Function

# AEGetSpecialHandler(\_:\_:\_:)

Gets a specified handler from a special handler dispatch table.

macOS 10.0+

``` source
func AEGetSpecialHandler(
    _ functionClass: AEKeyword,
    _ handler: UnsafeMutablePointer!,
    _ isSysHandler: Bool
) -> OSErr
```

## Parameters 

`functionClass`  

The keyword for the special handler to get. You can specify any of the constants described in Special Handler Callback Constants. See AEKeyword.

`handler`  

A universal procedure pointer. On return, a pointer to the specified special handler, if one exists that matches the value supplied in the `functionClass` parameter. See AEEventHandlerUPP.

`isSysHandler`  

Specifies the special handler dispatch table to get the handler from. Pass `TRUE` to get the handler from the system special handler dispatch table or `FALSE` to get the handler from your application’s special handler dispatch table. Use of the system special handler dispatch table is not recommended.

## Return Value

A result code. See Result Codes.

## Discussion

See also AEInstallSpecialHandler(_:_:_:) and AERemoveSpecialHandler(_:_:_:).

### Version-Notes

Thread safe starting in OS X v10.2.

In macOS, you should generally install all handlers in the application dispatch table. For Carbon applications running in Mac OS 8 or Mac OS 9, a special handler in the system dispatch table could reside in the system heap, where it would be available to other applications. However, this won’t work in macOS.

## See Also

### Managing Special Handler Dispatch Tables

func AEInstallSpecialHandler(AEKeyword, AEEventHandlerUPP!, Bool) -> OSErr

Installs a callback function in a special handler dispatch table.

func AERemoveSpecialHandler(AEKeyword, AEEventHandlerUPP!, Bool) -> OSErr

Removes a handler from a special handler dispatch table.

