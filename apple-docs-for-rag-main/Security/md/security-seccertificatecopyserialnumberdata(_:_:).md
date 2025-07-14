

- Security
-  SecCertificateCopySerialNumberData(\_:\_:) 

Function

# SecCertificateCopySerialNumberData(\_:\_:)

Returns the certificate’s serial number.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func SecCertificateCopySerialNumberData(
    _ certificate: SecCertificate,
    _ error: UnsafeMutablePointer?>?
) -> CFData?
```

## Parameters 

`certificate`  

The certificate from which to copy the serial number.

`error`  

A doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 pointer the function uses to return an error instance on failure. Set to `nil` to ignore any error.

## Return Value

The content of a DER-encoded integer (without the tag and length fields) for this certificate’s serial number.

## Discussion

In Objective-C, if the function returns an error free it with a call to CFRelease when you are done with it. If it returns data, you must free that as well.

