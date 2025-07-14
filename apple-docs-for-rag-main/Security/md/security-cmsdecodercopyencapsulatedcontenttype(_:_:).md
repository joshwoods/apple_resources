

- Security
-  CMSDecoderCopyEncapsulatedContentType(\_:\_:) 

Function

# CMSDecoderCopyEncapsulatedContentType(\_:\_:)

Obtains the object identifier for the encapsulated data of a signed message.

macOS 10.5+

``` source
func CMSDecoderCopyEncapsulatedContentType(
    _ cmsDecoder: CMSDecoder,
    _ eContentTypeOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`eContentTypeOut`  

On return, the object identifier for the encapsulated data in a signed message. Returns `NULL` if the message was not signed.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

In a signed message, the signed data consists of any type of content (referred to as the *encapsulated content*, because it is encapsulated in the signed data) plus the signature values. The content type of the encapsulated data is indicated by an object identifier. The default value for the OID is `id-data`, which indicates MIME-encoded content.

You cannot call this function until after you have called the `CMSDecoderFinalizeMessage` function.

