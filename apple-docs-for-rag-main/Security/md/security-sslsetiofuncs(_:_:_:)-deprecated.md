

- Security
-  SSLSetIOFuncs(\_:\_:\_:) Deprecated

Function

# SSLSetIOFuncs(\_:\_:\_:)

Specifies callback functions that perform the network I/O operations.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLSetIOFuncs(
    _ context: SSLContext,
    _ readFunc: SSLReadFunc,
    _ writeFunc: SSLWriteFunc
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`readFunc`  

A pointer to your read callback function. See SSLReadFunc for information on defining this function.

`writeFunc`  

A pointer to your write callback function. See SSLWriteFunc for information on defining this function.

## Return Value

A result code. See Secure Transport Result Codes.

## Mentioned in 

Using the Secure Socket Layer for Network Communication

## Discussion

Secure Transport calls your read and write callback functions to perform network I/O. You must define these functions before calling SSLSetIOFuncs(_:_:_:).

You must call SSLSetIOFuncs(_:_:_:) prior to calling the SSLHandshake(_:) function. SSLSetIOFuncs(_:_:_:) cannot be called while a session is active.

