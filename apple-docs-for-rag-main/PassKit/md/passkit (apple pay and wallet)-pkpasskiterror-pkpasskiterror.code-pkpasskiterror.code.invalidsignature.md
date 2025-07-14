

- PassKit (Apple Pay and Wallet)
- PKPassKitError
- PKPassKitError.Code
-  PKPassKitError.Code.invalidSignature 

Case

# PKPassKitError.Code.invalidSignature

Invalid pass signature.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
case invalidSignature
```

## Discussion

For example, the pass type identifier in the certificate and the pass do not match, or the certificate has expired or was revoked.

## See Also

### Error codes

case unknownError

Unknown error.

case invalidDataError

Invalid pass data.

case unsupportedVersionError

Unsupported pass version.

case notEntitledError

Error caused by absence of the required entitlements for the given operation.

