

- PassKit (Apple Pay and Wallet)
- PKSecureElementPass
-  primaryAccountNumberSuffix 

Instance Property

# primaryAccountNumberSuffix

A display-ready version of the primary account number.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
var primaryAccountNumberSuffix: String { get }
```

## Discussion

This property’s value is generally the last four or five digits of the primary account number, but can vary by issuer. The value isn’t related to primaryAccountIdentifier.

## See Also

### Getting the account attributes

var primaryAccountIdentifier: String

An opaque value that identifies the primary account number that funds the pass’s transactions.

