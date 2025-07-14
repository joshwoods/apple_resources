

- Security
-  SecCertificateCopySubjectSummary(\_:) 

Function

# SecCertificateCopySubjectSummary(\_:)

Returns a human-readable summary of a certificate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecCertificateCopySubjectSummary(_ certificate: SecCertificate) -> CFString?
```

## Parameters 

`certificate`  

The certificate object for which you wish to return a summary string.

## Return Value

A string that contains a human-readable summary of the contents of the certificate. In Objective-C, call the CFRelease function to release this object when you are finished with it. Returns `NULL` if the data passed in the `certificate` parameter is not a valid certificate object.

## Mentioned in 

Importing an Identity

Examining a Certificate

## Discussion

Because all the data in the string comes from the certificate, the string is in whatever language is used in the certificate.

## See Also

### Related Documentation

func SecCertificateCreateWithData(CFAllocator?, CFData) -> SecCertificate?

Creates a certificate object from a DER representation of a certificate.

