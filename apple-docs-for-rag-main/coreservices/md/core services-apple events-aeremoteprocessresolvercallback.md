

- Core Services
- Apple Events
-  AERemoteProcessResolverCallback 

Type Alias

# AERemoteProcessResolverCallback

Defines a pointer to a function the Apple Event Manager calls when the asynchronous execution of a remote process resolver completes, either due to success or failure, after a call to the `AERemoteProcessResolverScheduleWithRunLoop` function. Your callback function can use the reference passed to it to get the remote process information.

Mac Catalyst 13.0+macOS 10.3+

``` source
typealias AERemoteProcessResolverCallback = (AERemoteProcessResolverRef?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`ref`  

A reference of type AERemoteProcessResolverRef you can query to obtain the remote process information. Acquired from a previous call to AECreateRemoteProcessResolver(_:_:).

`info`  

An untyped pointer your application can use to pass information it needs when resolving remote processes. The application originally supplies this pointer in the AERemoteProcessResolverContext structure in the `ctx` parameter) when it calls the `AERemoteProcessResolverScheduleWithRunLoop` function.

## Return Value

Your callback routine should not return a value.

## See Also

### Callbacks

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

typealias OSLMarkProcPtr

Defines a pointer to an object marking callback function. Your object-marking function marks a specific Apple event object.

