

- Security
-  CMSDecoderCopyAllCerts(\_:\_:) 

Function

# CMSDecoderCopyAllCerts(\_:\_:)

Obtains an array of all of the certificates in a message.

macOS 10.5+

``` source
func CMSDecoderCopyAllCerts(
    _ cmsDecoder: CMSDecoder,
    _ certsOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`certsOut`  

On return, points to an array of `SecCertificateRef` objects. Returns `NULL` if the message does not contain any certificates (the message was encrypted but not signed); this is not considered an error. You must use the `CFRelease` function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A CMS message can contain arbitrary sets of certificates other than or in addition to those indicating the identity of signers. You can use this function to retrieve such certificates from a message. If the message was signed, it contains signer certificates. You can use the CMSDecoderGetNumSigners(_:_:) and CMSDecoderCopySignerCert(_:_:_:) functions to retrieve the certificates for a specific signer.

You cannot call this function until after you have called the CMSDecoderFinalizeMessage(_:) function.

## See Also

### Related Documentation

func CMSDecoderCopySignerCert(CMSDecoder, Int, UnsafeMutablePointer&lt;SecCertificate?>) -> OSStatus

Obtains the certificate of the specified signer of a CMS message.

func CMSEncoderAddSupportingCerts(CMSEncoder, CFTypeRef) -> OSStatus

Adds certificates to a message.

func CMSDecoderGetNumSigners(CMSDecoder, UnsafeMutablePointer&lt;Int>) -> OSStatus

Obtains the number of signers of a message.

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

func CMSDecoderFinalizeMessage(CMSDecoder) -> OSStatus

Indicates that there is no more data to decode.

