

- CryptoTokenKit
- TKBERTLVRecord
-  init(tag:records:) 

Initializer

# init(tag:records:)

Initializes a BER-TLV record with the specified tag and an array of TLV subrecords.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    tag: TKTLVTag,
    records: [TKTLVRecord]
)
```

## Parameters 

`tag`  

The tag field of the record.

`records`  

The TLV subrecords of the record.

## Return Value

A new TLV record containing the specified tag field and subrecords.

## See Also

### Creating TLV Records

init(tag: TKTLVTag, value: Data)

Initializes a BER-TLV record with the specified tag and value.

typealias TKTLVTag

The type used to identify TLV format tags.

