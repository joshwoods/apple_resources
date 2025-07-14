

- CryptoTokenKit
-  TKBERTLVRecord 

Class

# TKBERTLVRecord

An object that parses BER-encoded data and produces DER-encoded data for TLV records.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKBERTLVRecord
```

## Topics

### Creating TLV Records

init(tag: TKTLVTag, value: Data)

Initializes a BER-TLV record with the specified tag and value.

init(tag: TKTLVTag, records: [TKTLVRecord])

Initializes a BER-TLV record with the specified tag and an array of TLV subrecords.

typealias TKTLVTag

The type used to identify TLV format tags.

### Encoding Data

class func data(forTag: TKTLVTag) -> Data

Encodes a specified tag using BER-TLV tag encoding rules.

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

class TKCompactTLVRecord

An object that implements encoding using Compact-TLV encoding according to ISO 7816-4.

class TKSimpleTLVRecord

An object that implements encoding using Simple-TLV encoding according to ISO 7816-4.

