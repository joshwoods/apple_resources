

- PassKit (Apple Pay and Wallet)
- PKPassKitError
- PKPassKitError.Code
-  PKPassKitError.Code.notEntitledError 

Case

# PKPassKitError.Code.notEntitledError

Error caused by absence of the required entitlements for the given operation.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
case notEntitledError
```

## Discussion

Apps require appropriate entitlements to read, update or delete passes. To add these entitlements, enable the Wallet capabilities in Xcode.

## See Also

### Error codes

case unknownError

Unknown error.

case invalidDataError

Invalid pass data.

case unsupportedVersionError

Unsupported pass version.

case invalidSignature

Invalid pass signature.

