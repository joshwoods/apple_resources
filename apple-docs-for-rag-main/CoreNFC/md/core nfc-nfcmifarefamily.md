

- Core NFC
-  NFCMiFareFamily 

Enumeration

# NFCMiFareFamily

Identifiers for the MIFARE product families.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum NFCMiFareFamily
```

## Topics

### Product Families

case unknown

An identifier that indicates a compatible ISO14443 Type A tag.

case ultralight

An identifier that indicates the MIFARE Ultralight® product family.

case plus

An identifier that indicates the MIFARE Plus® product family.

case desfire

An identifier that indicates the MIFARE® DESFire® product family.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Tag Information

var mifareFamily: NFCMiFareFamily

The MIFARE product family identifier for the tag.

**Required**

var identifier: Data

The unique hardware identifier of the tag.

**Required**

var historicalBytes: Data?

The historical bytes extracted from an Answer To Select response.

**Required**

