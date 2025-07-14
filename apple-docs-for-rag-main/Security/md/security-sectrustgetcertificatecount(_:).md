

- Security
-  SecTrustGetCertificateCount(\_:) 

Function

# SecTrustGetCertificateCount(\_:)

Returns the number of certificates in an evaluated certificate chain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecTrustGetCertificateCount(_ trust: SecTrust) -> CFIndex
```

## Parameters 

`trust`  

The trust management object for the certificate that has been evaluated. Use the SecTrustCreateWithCertificates(_:_:_:) function to create a trust management object and the SecTrustEvaluateWithError(_:_:) function to evaluate the certificate chain.

## Return Value

The number of certificates in the certificate chain.

## Discussion

Call the SecTrustEvaluateWithError(_:_:) function before calling this function.

