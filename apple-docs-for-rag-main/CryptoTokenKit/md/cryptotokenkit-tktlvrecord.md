

- CryptoTokenKit
-  TKTLVRecord 

Class

# TKTLVRecord

The base class encapsulating a Tag-Length-Value record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTLVRecord
```

## Overview

The CryptoTokenKit framework provides the following concrete subclasses for various TLV record encodings:

- TKBERTLVRecord for BER-TLV encoding rules

- TKSimpleTLVRecord for Simple-TLV encoding according to ISO 7816-4

- TKCompactTLVRecord for Compact-TLV encoding according to ISO 7816-4

## Topics

### Creating Records

class func sequenceOfRecords(from: Data) -> [TKTLVRecord]?

Creates and returns an array of TLV records from the specified data.

convenience init?(from: Data)

Creates and returns a TLV record from by parsing the specified data.

### Accessing the Tag Field

var tag: TKTLVTag

The tag field of the record.

typealias TKTLVTag

The type used to identify TLV format tags.

### Accessing the Value Field

var value: Data

The value field of the record.

### Accessing Record Data

var data: Data

The record data, including the tag, length, and value fields.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TKBERTLVRecord
- TKCompactTLVRecord
- TKSimpleTLVRecord

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with Tag-Length-Value Records

class TKBERTLVRecord

An object that parses BER-encoded data and produces DER-encoded data for TLV records.

class TKCompactTLVRecord

An object that implements encoding using Compact-TLV encoding according to ISO 7816-4.

class TKSimpleTLVRecord

An object that implements encoding using Simple-TLV encoding according to ISO 7816-4.

