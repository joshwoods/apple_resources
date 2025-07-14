

- Security
-  CMSEncoderSetEncapsulatedContentTypeOID(\_:\_:) 

Function

# CMSEncoderSetEncapsulatedContentTypeOID(\_:\_:)

Specifies an object identifier for the encapsulated data of a signed message.

macOS 10.7+

``` source
func CMSEncoderSetEncapsulatedContentTypeOID(
    _ cmsEncoder: CMSEncoder,
    _ eContentTypeOID: CFTypeRef
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`eContentTypeOID`  

The object identifier for the encapsulated data in a signed message.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

In a signed message, the signed data consists of any type of content (referred to as the *encapsulated content*, because it is encapsulated in the signed data) plus the signature values. You can indicate the content type of the encapsulated data by specifying an object identifier (OID) in the `eContentTypeOID` parameter of this function, in the form of a Core Foundation string—`CFSTR("1.2.840.113549.1.7.1")`, for example.

The default value for the OID (used if this function is not called) is `id-data`. This is the normal encapsulated content type for applications such as S/MIME, which uses it to indicate MIME-encoded content. You can pass any value that is meaningful to your application. Examples of CMS OIDs are listed in http://www.imc.org/ietf-smime/other-smime-oids.asn.

If you do call this function, you must call it before the first call to the `CMSEncoderUpdateContent` function.

## See Also

### Related Documentation

func CMSDecoderCopyEncapsulatedContentType(CMSDecoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains the object identifier for the encapsulated data of a signed message.

func CMSEncoderUpdateContent(CMSEncoder, UnsafeRawPointer, Int) -> OSStatus

Feeds content bytes into the encoder.

func CMSEncoderCreate(UnsafeMutablePointer&lt;CMSEncoder?>) -> OSStatus

Creates a CMSEncoder reference.

func CMSEncoderCopyEncapsulatedContentType(CMSEncoder, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

Obtains the object identifier for the encapsulated data of a signed message.

