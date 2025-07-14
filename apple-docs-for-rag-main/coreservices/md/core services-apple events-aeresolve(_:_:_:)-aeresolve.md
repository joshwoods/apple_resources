

- Core Services
- Apple Events
-  AEResolve(\_:\_:\_:) 

Function

# AEResolve(\_:\_:\_:)

Resolves an object specifier.

macOS 10.0+

``` source
func AEResolve(
    _ objectSpecifier: UnsafePointer!,
    _ callbackFlags: Int16,
    _ theToken: UnsafeMutablePointer!
) -> OSErr
```

## Parameters 

`objectSpecifier`  

A pointer to the object specifier to resolve. See AEDesc.

`callbackFlags`  

A value that determines what additional assistance, if any, your application can give the Apple Event Manager when it parses the object specifier. The value is specified by adding the desired constants described in Callback Constants for the AEResolve Function. Most applications use `kAEIDoMinimum`.

`theToken`  

A pointer to a descriptor. On return, a token that identifies the Apple event objects specified by the `objectSpecifier` parameter. (Token is defined in AEDisposeToken(_:).)

Your object accessor functions may need to create many tokens to resolve a single object specifier; this parameter contains only the final token that identifies the requested Apple event object.

Whenever the `AEResolve` function returns final token to your event handler as the result of the resolving an object specifier passed to `AEResolve`, your application must deallocate the memory used by the token. If your application uses complex tokens, it must dispose of the token by calling AEDisposeToken(_:). If your application uses simple tokens, you can use either AEDisposeToken(_:) or AEDisposeDesc(_:). See AEDesc.

## Return Value

A result code. See Result Codes. The `AEResolve` function returns any result code returned by one of your application’s object accessor functions or object callback functions. For example, an object accessor function can return `errAENoSuchObject` (–1728) when it can’t find an Apple event object, or it can return more specific result codes. If any object accessor function or object callback function returns a result code other than `noErr` or `errAEEventNotHandled`, `AEResolve` immediately disposes of any existing tokens and returns. The result code it returns in this case is the result code returned by the object accessor function or the object callback function.

## Discussion

If an Apple event parameter consists of an object specifier, your handler for the event typically calls the `AEResolve` function to begin the process of resolving the object specifier.

The `AEResolve` function resolves the object specifier passed in the `objectSpecifier` parameter with the help of your object accessor functions, described in Apple Event Manager, and the object callback functions, described in Apple Event Manager.

For information on how to receive error information from the `AEResolve` function, see OSLGetErrDescProcPtr.

