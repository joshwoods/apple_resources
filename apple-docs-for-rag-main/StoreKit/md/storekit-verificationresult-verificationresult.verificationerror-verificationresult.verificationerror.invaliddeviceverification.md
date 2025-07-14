

- StoreKit
- VerificationResult
- VerificationResult.VerificationError
-  VerificationResult.VerificationError.invalidDeviceVerification 

Case

# VerificationResult.VerificationError.invalidDeviceVerification

An error that indicates the signed value wasn’t generated for the current device.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case invalidDeviceVerification
```

## See Also

### Error Codes

case invalidCertificateChain

An error indicating that the certificate chain is invalid.

case invalidEncoding

An error that indicates the signature, certificate chain, or other part of value uses invalid encoding.

case invalidSignature

An error that indicates that the signature didn’t match the header and payload.

case missingRequiredProperties

An error that indicates the header or payload are missing information that’s required to verify the signature.

case revokedCertificate

An error that indicates the certificate chain includes a revoked certificate.

