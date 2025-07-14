

- Security
-  SSLGetClientCertificateState(\_:\_:) Deprecated

Function

# SSLGetClientCertificateState(\_:\_:)

Retrieves the exchange status of the client certificate.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.3–10.15Deprecated

``` source
func SSLGetClientCertificateState(
    _ context: SSLContext,
    _ clientState: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`clientState`  

On return, a pointer to a value indicating the state of the client certificate exchange. See SSLClientCertificateState for a list of possible values.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

The value returned reflects the latest change in the state of the client certificate exchange. If either peer initiates a renegotiation attempt, Secure Transport resets the state to `kSSLClientCertNone`.

