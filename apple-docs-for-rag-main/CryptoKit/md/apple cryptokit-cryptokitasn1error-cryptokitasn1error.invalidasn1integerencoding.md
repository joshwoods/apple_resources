

- Apple CryptoKit
- CryptoKitASN1Error
-  CryptoKitASN1Error.invalidASN1IntegerEncoding 

Case

# CryptoKitASN1Error.invalidASN1IntegerEncoding

An ASN.1 integer doesn’t use the minimum number of bytes for its encoding.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case invalidASN1IntegerEncoding
```

## See Also

### Reporting errors

case invalidASN1Object

The format of the parsed ASN.1 object doesn’t match the format required for the data type being decoded.

case invalidFieldIdentifier

The ASN.1 tag for this field is invalid or unsupported.

case invalidObjectIdentifier

An ASN.1 object identifier is invalid.

case invalidPEMDocument

The string doesn’t parse as a PEM document.

case truncatedASN1Field

An ASN.1 field is truncated.

case unexpectedFieldType

The ASN.1 tag for the parsed field doesn’t match the required format.

case unsupportedFieldLength

The encoding used for the field length is unsupported.

