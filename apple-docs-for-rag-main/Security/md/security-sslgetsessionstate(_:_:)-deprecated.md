

- Security
-  SSLGetSessionState(\_:\_:) Deprecated

Function

# SSLGetSessionState(\_:\_:)

Retrieves the state of an SSL session.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
func SSLGetSessionState(
    _ context: SSLContext,
    _ state: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`state`  

On return, points to a constant that indicates the state of the SSL session. See SSLSessionState for possible values.

## Return Value

A result code. See Secure Transport Result Codes.

