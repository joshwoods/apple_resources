

- StoreKit
- VerificationResult
- VerificationResult.VerificationError
-  VerificationResult.VerificationError.invalidCertificateChain 

Case

# VerificationResult.VerificationError.invalidCertificateChain

An error indicating that the certificate chain is invalid.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case invalidCertificateChain
```

## Discussion

This error may occur if one or more certificates in the certiificate chain are expired or from an untrusted source.

## See Also

### Error Codes

case invalidDeviceVerification

An error that indicates the signed value wasn’t generated for the current device.

case invalidEncoding

An error that indicates the signature, certificate chain, or other part of value uses invalid encoding.

case invalidSignature

An error that indicates that the signature didn’t match the header and payload.

case missingRequiredProperties

An error that indicates the header or payload are missing information that’s required to verify the signature.

case revokedCertificate

An error that indicates the certificate chain includes a revoked certificate.

