

- Core Services
- Apple Events
-  AEInstallSpecialHandler(\_:\_:\_:) 

Function

# AEInstallSpecialHandler(\_:\_:\_:)

Installs a callback function in a special handler dispatch table.

macOS 10.0+

``` source
func AEInstallSpecialHandler(
    _ functionClass: AEKeyword,
    _ handler: AEEventHandlerUPP!,
    _ isSysHandler: Bool
) -> OSErr
```

## Parameters 

`functionClass`  

A value that specifies the type of handler to install. You can use any of the constants defined in Special Handler Callback Constants.

If there is already an entry in the specified special handler dispatch table for the value you specify in this parameter, it is replaced.

See AEKeyword.

`handler`  

A universal procedure pointer to the special handler to install. See AEEventHandlerUPP.

`isSysHandler`  

Specifies the special handler dispatch table to add the handler to. Pass `TRUE` to add the handler to the system special handler dispatch table or `FALSE` to add the handler to your application’s special handler dispatch table. Use of the system special handler dispatch table is not recommended.

## Return Value

A result code. See Result Codes.

## Discussion

An Apple event special handler dispatch table contains entries with a function class keyword, the address of the handler function that handles the Apple events indicated by the keyword, and a reference constant. Depending on which handlers you choose to install, a special handler dispatch table can have entries for any of the following:

- a predispatch handler (an Apple event handler that the Apple Event Manager calls immediately before it dispatches an Apple event)

- up to one each of the callback functions described in Apple Event Manager these functions, such as an object comparison function and an object-counting function, can be installed with `AEInstallSpecialHandler` or with the AEInstallObjectAccessor(_:_:_:_:_:) function

See also AEGetSpecialHandler(_:_:_:) and AERemoveSpecialHandler(_:_:_:).

### Version-Notes

Thread safe starting in OS X v10.2.

For Carbon applications running in Mac OS 8 or Mac OS 9, a handler in the system special handler dispatch table should reside in the system heap, where it may be available to other applications. If you put your system handler code in your application heap, be sure to use `AERemoveSpecialHandler` to remove the handler when your application quits. Otherwise, your handler will still have an entry in the system dispatch table with a pointer a handler that no longer exists. Another application may dispatch an Apple event that attempts to call your handler, leading to a system crash.

Your application should not install a handler in a system dispatch table with the goal that the handler will get called when other applications receive events—this won’t work in macOS.

## See Also

### Managing Special Handler Dispatch Tables

func AEGetSpecialHandler(AEKeyword, UnsafeMutablePointer&lt;AEEventHandlerUPP?>!, Bool) -> OSErr

Gets a specified handler from a special handler dispatch table.

func AERemoveSpecialHandler(AEKeyword, AEEventHandlerUPP!, Bool) -> OSErr

Removes a handler from a special handler dispatch table.

