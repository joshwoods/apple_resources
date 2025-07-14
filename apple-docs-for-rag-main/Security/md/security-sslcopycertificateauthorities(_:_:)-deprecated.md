

- Security
-  SSLCopyCertificateAuthorities(\_:\_:) Deprecated

Function

# SSLCopyCertificateAuthorities(\_:\_:)

Retrieves the current list of certification authorities.

macOS 10.5–10.15Deprecated

``` source
func SSLCopyCertificateAuthorities(
    _ context: SSLContext,
    _ certificates: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

No longer supported. Use Network.framework.

## Parameters 

`context`  

An SSL session context reference.

`certificates`  

On return, a pointer to a value of type `CFArrayRef`. This array contains values of type `SecCertificateRef` representing the current set of certification authorities (specified with the SSLSetCertificateAuthorities(_:_:_:) function). Returns a `NULL` array if SSLSetCertificateAuthorities(_:_:_:) has not been called. You must call the `CFRelease` function to release this array when you are finished with it.

## Return Value

A result code. See Secure Transport Result Codes.

## See Also

### Related Documentation

func SSLCopyDistinguishedNames(SSLContext, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the distinguished names of acceptable certification authorities.

Deprecated

