

- CryptoTokenKit
-  TKCompactTLVRecord 

Class

# TKCompactTLVRecord

An object that implements encoding using Compact-TLV encoding according to ISO 7816-4.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKCompactTLVRecord
```

## Topics

### Creating TLV Records

init(tag: UInt8, value: Data)

Initializes a TLV record with the specified tag and value.

## Relationships

### Inherits From

- TKTLVRecord

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with Tag-Length-Value Records

class TKTLVRecord

The base class encapsulating a Tag-Length-Value record.

class TKBERTLVRecord

An object that parses BER-encoded data and produces DER-encoded data for TLV records.

class TKSimpleTLVRecord

An object that implements encoding using Simple-TLV encoding according to ISO 7816-4.

