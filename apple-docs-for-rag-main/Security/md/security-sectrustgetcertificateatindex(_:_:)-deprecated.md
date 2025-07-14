

- Security
-  SecTrustGetCertificateAtIndex(\_:\_:) Deprecated

Function

# SecTrustGetCertificateAtIndex(\_:\_:)

Returns a specific certificate from the certificate chain used to evaluate trust.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.7–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
func SecTrustGetCertificateAtIndex(
    _ trust: SecTrust,
    _ ix: CFIndex
) -> SecCertificate?
```

## Parameters 

`trust`  

The trust management object for the certificate that has been evaluated. Use the SecTrustCreateWithCertificates(_:_:_:) function to create a trust management object and the SecTrustEvaluateWithError(_:_:) function to evaluate the certificate chain.

`ix`  

The index number of the requested certificate. Index numbers start at 0 for the leaf certificate and end at the anchor (or the last certificate if no anchor was found). Use the SecTrustGetCertificateCount(_:) function to get the total number of certificates in the chain.

## Return Value

A certificate object for the requested certificate.

## Discussion

Call the SecTrustEvaluateWithError(_:_:) function before calling this function.

