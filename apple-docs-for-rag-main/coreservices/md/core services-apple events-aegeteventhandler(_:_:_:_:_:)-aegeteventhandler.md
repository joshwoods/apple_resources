

- Core Services
- Apple Events
-  AEGetEventHandler(\_:\_:\_:\_:\_:) 

Function

# AEGetEventHandler(\_:\_:\_:\_:\_:)

Gets an event handler from an Apple event dispatch table.

macOS 10.0+

``` source
func AEGetEventHandler(
    _ theAEEventClass: AEEventClass,
    _ theAEEventID: AEEventID,
    _ handler: UnsafeMutablePointer!,
    _ handlerRefcon: UnsafeMutablePointer!,
    _ isSysHandler: Bool
) -> OSErr
```

## Parameters 

`theAEEventClass`  

The event class for the desired handler. See AEEventClass.

`theAEEventID`  

The event ID for the desired handler. See AEEventID.

`handler`  

A universal procedure pointer. On return, a pointer to the specified handler, if a dispatch table entry exists that exactly matches the values supplied in the parameters `theAEEventClass` and `theAEEventID`.

If you use the `typeWildCard` constant for either or both of these parameters, `AEGetEventHandler` will return an error unless an entry exists that specifies `typeWildCard` in exactly the same way. For example, if you specify `typeWildCard` in both the `theAEEventClass` parameter and the `theAEEventID` parameter, the Apple Event Manager will not return the first handler for any event class and event ID in the dispatch table; instead, it will only return a handler if an entry exists that specifies type `typeWildCard` for both the event class and the event ID.

For an explanation of wildcard values, see the Discussion section for AEInstallEventHandler(_:_:_:_:_:).

See AEEventHandlerUPP.

`handlerRefcon`  

A pointer to a reference constant. On return, the reference constant from the dispatch table entry for the specified handler. The reference constant may have a value of 0.

`isSysHandler`  

Specifies the Apple event dispatch table to get the handler from. Pass `TRUE` to get the handler from the system dispatch table or `FALSE` to get the handler from your application’s dispatch table. See Version Notes for related information.

## Return Value

A result code. See Result Codes.

## Discussion

Thread safe starting in OS X v10.2.

Your application should not install a handler in a system dispatch table with the goal that the handler will get called when other applications receive events—this won’t work in macOS. For more information, see The System Dispatch Table in Apple Event Dispatching in Apple Events Programming Guide.

In Mac OS 7.1 through 9.x and macOS version v10.2 and later, `AEGetEventHandler` returns `errAEHandlerNotInstalled` when there’s not an exact match, even if a wildcard handler is installed that could handle the event. macOS version v10.0.x and v10.1.x will return the wildcard handler.

## See Also

### Managing Apple Event Dispatch Tables

func AEInstallEventHandler(AEEventClass, AEEventID, AEEventHandlerUPP!, SRefCon!, Bool) -> OSErr

Adds an entry for an event handler to an Apple event dispatch table.

func AERemoveEventHandler(AEEventClass, AEEventID, AEEventHandlerUPP!, Bool) -> OSErr

Removes an event handler entry from an Apple event dispatch table.

