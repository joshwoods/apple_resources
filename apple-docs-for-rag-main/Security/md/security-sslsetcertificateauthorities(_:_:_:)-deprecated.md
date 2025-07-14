

- Security
-  SSLSetCertificateAuthorities(\_:\_:\_:) Deprecated

Function

# SSLSetCertificateAuthorities(\_:\_:\_:)

Adds one or more certificates to a server’s list of certification authorities (CAs) acceptable for client authentication.

macOS 10.5–10.15Deprecated

``` source
func SSLSetCertificateAuthorities(
    _ context: SSLContext,
    _ certificateOrArray: CFTypeRef,
    _ replaceExisting: Bool
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`certificateOrArray`  

A value of type `SecCertificateRef`, or a value of type `CFArray` containing an array of `SecCertificateRef` values, representing one or more certificates to be added to the server’s list of acceptable certification authorities (CAs).

`replaceExisting`  

A Boolean value specifying whether to replace or append the current set of certification authorities. If this value is `true`, the specified certificates replace the existing list of acceptable CAs, if any. If `false`, the specified certificates are appended to the existing list of.

## Return Value

A result code. See Secure Transport Result Codes. Returns errSecParam if this function is called for a session that is configured as a client, or when a session is active.

## Discussion

Each successive call to this function with the `replaceExisting` parameter set to false results in accumulation of additional certification authorities. To see the current set of certification authorities, call the SSLCopyCertificateAuthorities(_:_:) function.

## See Also

### Related Documentation

func SSLCopyDistinguishedNames(SSLContext, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the distinguished names of acceptable certification authorities.

Deprecated

