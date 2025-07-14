

- Core Services
- Apple Events
-  AECoerceDescProcPtr 

Type Alias

# AECoerceDescProcPtr

Defines a pointer to a function that coerces data stored in a descriptor. Your descriptor coercion callback function coerces the data from the passed descriptor to the specified type, returning the coerced data in a second descriptor.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AECoerceDescProcPtr = (UnsafePointer?, DescType, SRefCon?, UnsafeMutablePointer?) -> OSErr
```

## Parameters 

`fromDesc`  

A pointer to the descriptor that contains the data to coerce. See AEDesc.

`toType`  

The desired descriptor type for the resulting descriptor. For a list of AppleScript’s predefined descriptor types, see Descriptor Type Constants. See DescType.

`handlerRefcon`  

A reference constant that is stored in the coercion dispatch table entry for the handler. The Apple Event Manager passes this value to the handler each time it calls it. The reference constant may have a value of 0.

`toDesc`  

A pointer to a descriptor where your coercion routine must store the descriptor that contains the coerced data. See AEDesc.

## Return Value

A result code. See Result Codes. Your handler should return `noErr` if it successfully handled the coercion, `errAECoercionFailed` if it can’t handle the coercion and it wants the Apple Event Manager to continue dispatching to other coercion handlers, or a nonzero result code otherwise.

## Discussion

Your coercion handler should coerce the data to the desired descriptor type and return the resulting data in the descriptor specified by the `result` parameter.

To provide a pointer to your descriptor coercion callback function, you create a universal procedure pointer (UPP) of type AECoerceDescUPP, using the function NewAECoerceDescUPP(_:). You can do so with code like the following:

AECoerceDescUPP MyCoerceDescUPP;
MyCoerceDescUPP = NewAECoerceDescUPP (&amp;MyCoerceDescCallback)

You can then pass the UPP` MyCoerceDescUPP` as a parameter to any function that installs or removes a coercion handler, such as AEInstallCoercionHandler(_:_:_:_:_:_:). If your application installs the same coercion handler to coerce more than one type of data, you can use the same UPP to install the handler multiple times.

If you wish to call your descriptor coercion callback function directly, you can use the InvokeAECoerceDescUPP(_:_:_:_:_:) function.

After you are finished with a descriptor coercion callback function, and have removed it with the AERemoveCoercionHandler(_:_:_:_:) function, you can dispose of the UPP with the DisposeAECoerceDescUPP(_:) function. However, don’t dispose of the UPP if any remaining coercion handler uses it or if you plan to install the coercion handler again.

## See Also

### Callbacks

typealias AERemoteProcessResolverCallback

Defines a pointer to a function the Apple Event Manager calls when the asynchronous execution of a remote process resolver completes, either due to success or failure, after a call to the `AERemoteProcessResolverScheduleWithRunLoop` function. Your callback function can use the reference passed to it to get the remote process information.

typealias AEDisposeExternalProcPtr

Defines a pointer to a function the Apple Event Manager calls to dispose of a descriptor created by the `AECreateDescFromExternalPtr` function. Your callback function disposes of the buffer you originally passed to that function.

typealias AECoercePtrProcPtr

Defines a pointer to a function that coerces data stored in a buffer. Your pointer coercion callback routine coerces the data from the passed buffer to the specified type, returning the coerced data in a descriptor.

typealias AEEventHandlerProcPtr

Defines a pointer to a function that handles one or more Apple events. Your Apple event handler function performs any action requested by the Apple event, adds parameters to the reply Apple event if appropriate (possibly including error information), and returns a result code.

typealias OSLAccessorProcPtr

Your object accessor function either finds elements or properties of an Apple event object.

typealias OSLAdjustMarksProcPtr

Defines a pointer to an adjust marks callback function. Your adjust marks function unmarks objects previously marked by a call to your marking function.

typealias OSLCompareProcPtr

Defines a pointer to an object comparison callback function. Your object comparison function compares one Apple event object to another or to the data for a descriptor.

typealias OSLCountProcPtr

Defines a pointer to an object counting callback function. Your object counting function counts the number of Apple event objects of a specified class in a specified container object.

typealias OSLDisposeTokenProcPtr

Defines a pointer to a dispose token callback function. Your dispose token function, required only if you use a complex token format, disposes of the specified token.

typealias OSLGetErrDescProcPtr

Defines a pointer to an error descriptor callback function. Your error descriptor callback function supplies a pointer to an address where the Apple Event Manager can store the current descriptor if an error occurs during a call to the `AEResolve` function.

typealias OSLGetMarkTokenProcPtr

Defines a pointer to a mark token callback function. Your mark token function returns a mark token.

typealias OSLMarkProcPtr

Defines a pointer to an object marking callback function. Your object-marking function marks a specific Apple event object.

