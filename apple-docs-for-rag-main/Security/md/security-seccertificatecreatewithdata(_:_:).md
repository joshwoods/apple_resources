

- Security
-  SecCertificateCreateWithData(\_:\_:) 

Function

# SecCertificateCreateWithData(\_:\_:)

Creates a certificate object from a DER representation of a certificate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecCertificateCreateWithData(
    _ allocator: CFAllocator?,
    _ data: CFData
) -> SecCertificate?
```

## Parameters 

`allocator`  

The `CFAllocator` object you wish to use to allocate the certificate object. Pass `NULL` to use the default allocator.

`data`  

A DER (Distinguished Encoding Rules) representation of an X.509 certificate.

## Return Value

The newly created certificate object. In Objective-C, call the CFRelease function to release this object when you are finished with it. Returns `nil` if the data passed in the `data` parameter is not a valid DER-encoded X.509 certificate.

## Mentioned in 

Storing a DER-Encoded X.509 Certificate

## Discussion

The certificate object returned by this function is used as input to other functions in the API.

