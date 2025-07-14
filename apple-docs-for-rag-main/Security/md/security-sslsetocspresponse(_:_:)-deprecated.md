

- Security
-  SSLSetOCSPResponse(\_:\_:) Deprecated

Function

# SSLSetOCSPResponse(\_:\_:)

Sets the OCSP response for the given SSL session.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.13–10.15Deprecated

``` source
func SSLSetOCSPResponse(
    _ context: SSLContext,
    _ response: CFData
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

A session context.

`response`  

A non-`NULL` CFData instance containing the bytes of the OCSP response.

## Return Value

A result code. See Secure Transport Result Codes.

