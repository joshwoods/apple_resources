

- Security
-  SecCertificateCopyEmailAddresses(\_:\_:) 

Function

# SecCertificateCopyEmailAddresses(\_:\_:)

Retrieves the email addresses for the subject of a certificate.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.5+tvOS 10.2+visionOS 1.0+watchOS 3.2+

``` source
func SecCertificateCopyEmailAddresses(
    _ certificate: SecCertificate,
    _ emailAddresses: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`certificate`  

The certificate object from which to retrieve the email addresses.

`emailAddresses`  

On return, an array of zero or more `CFStringRef` elements, each containing one email address found in the certificate subject. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Not every certificate subject includes an email address. If the function does not find any email addresses, it returns a `CFArrayRef` object with zero elements in the array.

