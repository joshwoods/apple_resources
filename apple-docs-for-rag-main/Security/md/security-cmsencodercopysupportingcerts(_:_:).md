

- Security
-  CMSEncoderCopySupportingCerts(\_:\_:) 

Function

# CMSEncoderCopySupportingCerts(\_:\_:)

Obtains the certificates added to a message with `CMSEncoderAddSupportingCerts`.

macOS 10.5+

``` source
func CMSEncoderCopySupportingCerts(
    _ cmsEncoder: CMSEncoder,
    _ certsOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`certsOut`  

On return, points to a CFArray of `SecCertificateRef` objects. You must use the `CFRelease` function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

A CMS message can contain arbitrary sets of certificates other than or in addition to those indicating the identity of signers. You can use this function to obtain any such certificates added with the `CMSEncoderAddSupportingCerts` function. If `CMSEncoderAddSupportingCerts` has not been called, this function returns a `NULL` value for `certsOut`. Note that this function does not return the signing certificates, if any.

## See Also

### Related Documentation

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

func CMSEncoderAddSupportingCerts(CMSEncoder, CFTypeRef) -> OSStatus

Adds certificates to a message.

