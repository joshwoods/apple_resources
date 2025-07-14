

- Security
-  SSLCopyALPNProtocols(\_:\_:) Deprecated

Function

# SSLCopyALPNProtocols(\_:\_:)

Gets the list of supported application layer protocols.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15Deprecated

``` source
func SSLCopyALPNProtocols(
    _ context: SSLContext,
    _ protocols: UnsafeMutablePointer?>
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

The session context.

`protocols`  

A pointer the function uses to return an array of ASCII-encoded strings representing the supported protocols, such as http/1.1. See RFC 7301 for more details.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

You must set the `protocols` parameter to `NULL` on input, or the operation fails. If the function has data to provide, it allocates memory for an array and returns it using `protocols`. Otherwise, `protocols` remains `NULL` on output.

