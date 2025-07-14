

- HealthKit
- HKVerifiableClinicalRecord
-  jwsRepresentation Deprecated

Instance Property

# jwsRepresentation

A raw representation of the SMART Health Card’s contents.

iOS 15.0–15.4DeprecatediPadOS 15.0–15.4DeprecatedMac Catalyst 15.0–15.4DeprecatedmacOS 13.0+visionOS 1.0–1.0Deprecated

``` source
var jwsRepresentation: Data { get }
```

Deprecated

Use dataRepresentation instead.

## Discussion

This property contains a JSON Web Signature (JWS) Compact Serialization of the card. The data is cryptographically signed by the issuer, and compressed.

Important

To ensure that the data is authentic and that no one has tampered with it, decompress the data and then use a public key from the issuer to verify their signature.

## See Also

### Accessing the Raw Payload

var dataRepresentation: Data

A raw representation of the record’s data.

