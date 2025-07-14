

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassConfiguration
-  issuerIdentifier 

Instance Property

# issuerIdentifier

An opaque value for the configuration.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+

``` source
var issuerIdentifier: String? { get set }
```

## Discussion

Important

This property’s value is unique for each issuer. This property is available only to developers who work with Apple to enable this functionality.

## See Also

### Managing the issuer identity

var localizedDescription: String?

The configuration’s localized description.

