

- Security
-  SecCertificateCopyCommonName(\_:\_:) 

Function

# SecCertificateCopyCommonName(\_:\_:)

Retrieves the common name of the subject of a certificate.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.5+tvOS 10.2+visionOS 1.0+watchOS 3.2+

``` source
func SecCertificateCopyCommonName(
    _ certificate: SecCertificate,
    _ commonName: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`certificate`  

The certificate object from which to retrieve the common name.

`commonName`  

On return, points to the common name. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

