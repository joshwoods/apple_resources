

- Security
-  SSLSetDiffieHellmanParams(\_:\_:\_:) Deprecated

Function

# SSLSetDiffieHellmanParams(\_:\_:\_:)

Specifies Diffie-Hellman parameters for a given context.

macOS 10.2–10.15Deprecated

``` source
func SSLSetDiffieHellmanParams(
    _ context: SSLContext,
    _ dhParams: UnsafeRawPointer?,
    _ dhParamsLen: Int
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`dhParams`  

A pointer to a buffer containing the Diffie-Hellman parameters in Open SSL DER format.

`dhParamsLen`  

A value representing the size of the buffer pointed to by the `dhParams` parameter.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

You can use this function to specify a set of Diffie-Hellman parameters to be used by Secure Transport for a specific session. Use of this function is optional. If Diffie-Hellman ciphers are allowed, the server and client negotiate a Diffie-Hellman cipher, and this function has not been called, then secure transport calculates a set of process wide parameters. However, that process can take as long as 30 seconds. Diffie-Hellman ciphers are enabled by default. See SSLSetEnabledCiphers(_:_:_:).

In SSL/TLS, Diffie-Hellman parameters are always specified by the server. Therefore, this function can be called only by the server side of the connection.

You can use the SSLGetDiffieHellmanParams(_:_:_:) function to retrieve Diffie-Hellman parameters specified in an earlier call to SSLSetDiffieHellmanParams(_:_:_:).

