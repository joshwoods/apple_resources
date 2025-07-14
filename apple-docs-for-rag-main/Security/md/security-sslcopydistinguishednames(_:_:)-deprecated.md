

- Security
-  SSLCopyDistinguishedNames(\_:\_:) Deprecated

Function

# SSLCopyDistinguishedNames(\_:\_:)

Retrieves the distinguished names of acceptable certification authorities.

iOS 5.0–13.0DeprecatediPadOS 5.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.15Deprecated

``` source
func SSLCopyDistinguishedNames(
    _ context: SSLContext,
    _ names: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`names`  

On return, an array of `CFDataRef` objects, each representing one DER-encoded relative distinguished name of an acceptable certification authority. You must call the `CFRelease` function to release this array when you are finished with it.

## Return Value

A result code. See Secure Transport Result Codes.

## Discussion

The list of distinguished names is provided by the server if the context reference represents a client; if the context reference represents a server, the list of distinguished names is specified with the SSLSetCertificateAuthorities(_:_:_:) function.

The array retrieved by this function is suitable for use in finding a client identity (that is, a certificate and associated private key) that matches a server’s requirements.

## See Also

### Related Documentation

func SSLSetCertificateAuthorities(SSLContext, CFTypeRef, Bool) -> OSStatus

Adds one or more certificates to a server’s list of certification authorities (CAs) acceptable for client authentication.

Deprecated

func SSLCopyCertificateAuthorities(SSLContext, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the current list of certification authorities.

Deprecated

