

- CryptoTokenKit
- TKCompactTLVRecord
-  init(tag:value:) 

Initializer

# init(tag:value:)

Initializes a TLV record with the specified tag and value.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    tag: UInt8,
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

