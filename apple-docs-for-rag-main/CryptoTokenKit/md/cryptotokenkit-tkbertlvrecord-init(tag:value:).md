

- CryptoTokenKit
- TKBERTLVRecord
-  init(tag:value:) 

Initializer

# init(tag:value:)

Initializes a BER-TLV record with the specified tag and value.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    tag: TKTLVTag,
    value: Data
)
```

## Parameters 

`tag`  

The tag field of the record.

`value`  

The value field of the record.

## Return Value

A new TLV record containing the specified tag and value fields.

## See Also

### Creating TLV Records

init(tag: TKTLVTag, records: [TKTLVRecord])

Initializes a BER-TLV record with the specified tag and an array of TLV subrecords.

typealias TKTLVTag

The type used to identify TLV format tags.

