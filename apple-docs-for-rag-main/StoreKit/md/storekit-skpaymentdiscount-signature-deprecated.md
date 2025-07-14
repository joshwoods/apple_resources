

- StoreKit
- SKPaymentDiscount
-  signature Deprecated

Instance Property

# signature

A string representing the properties of a specific promotional offer, cryptographically signed.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var signature: String { get }
```

Deprecated

Create a Product.PurchaseOption.promotionalOffer to use in Product.purchase(confirmIn:options:)

## Mentioned in 

Implementing promotional offers in your app

## Discussion

The signature is a string signed with your private key that represents the properties of a specific promotional offer. To keep your private key secure, generate the signature on a server.

Generate the signature using the Elliptic Curve Digital Signature Algorithm (ECDSA) with SHA 256. For more information, see Generating a signature for promotional offers.

## See Also

### Validating the Discount

var nonce: UUID

A universally unique ID (UUID) value that you define.

Deprecated

var timestamp: NSNumber

The date and time of the signature’s creation in milliseconds, formatted in Unix epoch time.

Deprecated

