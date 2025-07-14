

- Security
-  SSLSetError(\_:\_:) Deprecated

Function

# SSLSetError(\_:\_:)

Sets the status of a session context.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15Deprecated

``` source
func SSLSetError(
    _ context: SSLContext,
    _ status: OSStatus
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

A session context.

`status`  

A status result for the context, not to be confused with the return result of this function call. See Secure Transport Result Codes.

## Return Value

A result code that represents the outcome of this function call, not to be confused with the `status` parameter. See Secure Transport Result Codes.

## Discussion

Call this function after handling the steps of an SSL handshake, such as server certificate validation.

