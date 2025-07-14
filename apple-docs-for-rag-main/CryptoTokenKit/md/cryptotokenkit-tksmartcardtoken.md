

- CryptoTokenKit
-  TKSmartCardToken 

Class

# TKSmartCardToken

A representation of a smart card based cryptographic token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKSmartCardToken
```

## Mentioned in 

Authenticating Users with a Cryptographic Token

## Topics

### Creating Smart Card Tokens

init(smartCard: TKSmartCard, aid: Data?, instanceID: String, tokenDriver: TKSmartCardTokenDriver)

Initializes a smart card token with the specified smart card, application identifier, and token driver.

### Accessing the Application Identifier

var aid: Data?

The ISO 7816-4 application identifiers of the Smart Card.

### Accessing Smart Cards

class TKSmartCard

A representation of a smart card.

### Working with Tag-Length-Value Records

class TKTLVRecord

The base class encapsulating a Tag-Length-Value record.

class TKBERTLVRecord

An object that parses BER-encoded data and produces DER-encoded data for TLV records.

class TKCompactTLVRecord

An object that implements encoding using Compact-TLV encoding according to ISO 7816-4.

class TKSimpleTLVRecord

An object that implements encoding using Simple-TLV encoding according to ISO 7816-4.

## Relationships

### Inherits From

- TKToken

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Smart Card App Extensions

Authenticating Users with a Cryptographic Token

Grant access to user accounts and the keychain by creating a smart card app extension.

Configuring Smart Card Authentication

Set preferences for smart card authentication operations, including those on managed devices.

class TKSmartCardTokenDriver

The driver that acts as an entry point for smart card app extensions.

class TKSmartCardTokenSession

A token session that is based on a smart card token.

