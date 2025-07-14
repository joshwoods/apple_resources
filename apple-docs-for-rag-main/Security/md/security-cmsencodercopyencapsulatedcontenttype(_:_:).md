

- Security
-  CMSEncoderCopyEncapsulatedContentType(\_:\_:) 

Function

# CMSEncoderCopyEncapsulatedContentType(\_:\_:)

Obtains the object identifier for the encapsulated data of a signed message.

macOS 10.5+

``` source
func CMSEncoderCopyEncapsulatedContentType(
    _ cmsEncoder: CMSEncoder,
    _ eContentTypeOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the `CMSEncoderCreate` function.

`eContentTypeOut`  

On return, points to the object identifier for the encapsulated data in the signed message.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

In a signed message, the signed data consists of any type of data (the *encapsulated content*) plus the signature values. This function returns the object identifier (OID) of the encapsulated content as it was specified with the `CMSEncoderSetEncapsulatedContentType` function.

If the `CMSEncoderSetEncapsulatedContentType` function has not been called for this message, this function returns a `NULL` pointer.

