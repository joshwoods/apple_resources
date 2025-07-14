

- Security
-  SSLGetSessionOption(\_:\_:\_:) Deprecated

Function

# SSLGetSessionOption(\_:\_:\_:)

Indicates the current setting of Secure Sockets Layer (SSL) session options.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.15Deprecated

``` source
func SSLGetSessionOption(
    _ context: SSLContext,
    _ option: SSLSessionOption,
    _ value: UnsafeMutablePointer
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

On return, `true` if the option is enabled, or `false` otherwise.

## Return Value

A result code. See Secure Transport Result Codes.

