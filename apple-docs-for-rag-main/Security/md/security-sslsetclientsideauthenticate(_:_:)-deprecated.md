

- Security
-  SSLSetClientSideAuthenticate(\_:\_:) Deprecated

Function

# SSLSetClientSideAuthenticate(\_:\_:)

Specifies the requirements for client-side authentication.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLSetClientSideAuthenticate(
    _ context: SSLContext,
    _ auth: SSLAuthenticate
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`auth`  

A flag setting the requirements for client-side authentication. See SSLAuthenticate for possible values.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

This function can be called only by servers. Use of this function is optional. The default authentication requirement is SSLAuthenticate.neverAuthenticate. This function may be called only when no session is active.

