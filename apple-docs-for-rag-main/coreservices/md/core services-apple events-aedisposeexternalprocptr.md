

- Core Services
- Apple Events
-  AEDisposeExternalProcPtr 

Type Alias

# AEDisposeExternalProcPtr

Defines a pointer to a function the Apple Event Manager calls to dispose of a descriptor created by the `AECreateDescFromExternalPtr` function. Your callback function disposes of the buffer you originally passed to that function.

Mac Catalyst 13.0+macOS 10.2+

``` source
typealias AEDisposeExternalProcPtr = (UnsafeRawPointer?, Size, SRefCon?) -> Void
```

## Parameters 

`dataPtr`  

A pointer to the data to be disposed of. The data must be immutable and must not be freed until this callback function is called.

`dataLength`  

The length, in bytes, of the data in the `dataPtr` parameter.

`refcon`  

A reference constant, supplied by your application in its original call to AECreateDescFromExternalPtr(_:_:_:_:_:_:). The Apple Event Manager passes this value to your dispose function each time it calls it. The reference constant may have a value of 0.

## Return Value

Your callback routine should not return a value.

## Discussion

Your application must provide a universal procedure pointer to a dispose function as a parameter to the AECreateDescFromExternalPtr(_:_:_:_:_:_:) function.

To provide a pointer to your dispose callback function, you create a universal procedure pointer (UPP) of type `AEDisposeExternalProcPtr`, using the function NewAEDisposeExternalUPP(_:). You can do so with code like the following:

AEDisposeExternalProcPtr MyDisposeCallbackUPP;
MyDisposeCallbackUPP = NewAEDisposeExternalUPP (&amp;MyAEDisposeExternalCallback);

You can then pass the UPP `MyDisposeCallbackUPP` as a parameter to the `AECreateDescFromExternalPtr` function.

If you wish to call your dispose callback function directly, you can use the InvokeAEDisposeExternalUPP(_:_:_:_:) function.

After you are finished with your dispose callback function, you can dispose of the UPP with the DisposeAEDisposeExternalUPP(_:) function. However, if you will use the same dispose function in subsequent calls to `AECreateDescFromExternalPtr`, you can reuse the same UPP, rather than dispose of it and later create a new UPP.

## See Also

### Callbacks

typealias AERemoteProcessResolverCallback

Defines a pointer to a function the Apple Event Manager calls when the asynchronous execution of a remote process resolver completes, either due to success or failure, after a call to the `AERemoteProcessResolverScheduleWithRunLoop` function. Your callback function can use the reference passed to it to get the remote process information.

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

typealias OSLMarkProcPtr

Defines a pointer to an object marking callback function. Your object-marking function marks a specific Apple event object.

