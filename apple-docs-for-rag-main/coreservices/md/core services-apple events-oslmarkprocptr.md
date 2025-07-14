

- Core Services
- Apple Events
-  OSLMarkProcPtr 

Type Alias

# OSLMarkProcPtr

Defines a pointer to an object marking callback function. Your object-marking function marks a specific Apple event object.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias OSLMarkProcPtr = (UnsafePointer?, UnsafePointer?, Int) -> OSErr
```

## Parameters 

`dToken`  

A pointer to the token for the Apple event object to be marked. (Token is defined in AEDisposeToken(_:). See AEDesc.

`markToken`  

A pointer to the mark token used to mark the Apple event object. See AEDesc.

`index`  

The number of times your `MyMarkCallback` function has been called for the current mark token (that is, the number of Apple event objects that have so far passed the test, including the element to be marked).

## Return Value

A result code. See Result Codes. Your object marking function should return `noErr` if it successfully marks the Apple event object and `errAEEventNotHandled` if it fails to mark the object. When the Apple Event Manager gets an error result of `errAEEventNotHandled` after calling an object marking function, it attempts to get mark the object by calling the equivalent system object marking function.

## Discussion

To mark an Apple event object using the current mark token, the Apple Event Manager calls the object-marking function provided by your application. In addition to marking the specified object, your `MyMarkCallback` function should record the mark count for each object that it marks. The mark count recorded for each marked object allows your application to determine which of a set of marked tokens pass a test, as described in the Discussion section for the OSLAdjustMarksProcPtr function.

To provide a pointer to your mark callback function, you create a universal procedure pointer (UPP) of type OSLMarkUPP, using the function NewOSLMarkUPP(_:). You can do so with code like the following:

OSLMarkUPP MyMarkUPP;
MyMarkUPP = NewOSLMarkUPP (&amp;MyMarkCallback)

You can then pass the UPP `MyMarkUPP` as a parameter to the AESetObjectCallbacks(_:_:_:_:_:_:_:) function or the AEInstallSpecialHandler(_:_:_:) function.

If you wish to call your mark callback function directly, you can use the InvokeOSLMarkUPP(_:_:_:_:) function.

After you are finished with your mark callback function, you can dispose of the UPP with the DisposeOSLMarkUPP(_:) function. However, if you will use the same mark function in subsequent calls to the function `AESetObjectCallbacks` or the function `AEInstallSpecialHandler`, you can reuse the same UPP, rather than dispose of it and later create a new UPP.

## See Also

### Callbacks

typealias AERemoteProcessResolverCallback

Defines a pointer to a function the Apple Event Manager calls when the asynchronous execution of a remote process resolver completes, either due to success or failure, after a call to the `AERemoteProcessResolverScheduleWithRunLoop` function. Your callback function can use the reference passed to it to get the remote process information.

typealias AEDisposeExternalProcPtr

Defines a pointer to a function the Apple Event Manager calls to dispose of a descriptor created by the `AECreateDescFromExternalPtr` function. Your callback function disposes of the buffer you originally passed to that function.

typealias AECoerceDescProcPtr

Defines a pointer to a function that coerces data stored in a descriptor. Your descriptor coercion callback function coerces the data from the passed descriptor to the specified type, returning the coerced data in a second descriptor.

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

