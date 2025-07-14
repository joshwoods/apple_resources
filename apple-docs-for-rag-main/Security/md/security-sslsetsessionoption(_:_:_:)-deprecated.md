

- Security
-  SSLSetSessionOption(\_:\_:\_:) Deprecated

Function

# SSLSetSessionOption(\_:\_:\_:)

Specifies options for a specific session.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.15Deprecated

``` source
func SSLSetSessionOption(
    _ context: SSLContext,
    _ option: SSLSessionOption,
    _ value: Bool
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`option`  

An SSL session option. Possible values are listed in SSLSessionOption.

`value`  

Set to true to enable the option, or false to disable it.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

This function must be called prior to the SSLHandshake(_:) function; consequently, this function can be called only when no session is active.

