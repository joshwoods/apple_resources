

- HealthKit
- HKVerifiableClinicalRecord
-  dataRepresentation 

Instance Property

# dataRepresentation

A raw representation of the record’s data.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS 1.0+

``` source
var dataRepresentation: Data { get }
```

## Discussion

The data’s format varies based on its sourceType:

SMART Health Card  
The raw representation corresponds to the compact JSON Web Signatures (JWS) serialization. For more information, see SMART Health Card Framework.

EU-DCC Records  
The raw representation corresponds to the CBOR Web Tokens (CWT) of the Electronic Health Certificate (HCERT). For more information, see Electronic Health Certificates.

Important

To ensure that the data is authentic and that no one has tampered with it, decompress the data and then use a public key from the issuer to verify their signature.

## See Also

### Accessing the Raw Payload

var jwsRepresentation: Data

A raw representation of the SMART Health Card’s contents.

Deprecated

