

- CryptoTokenKit
- TKBERTLVRecord
-  data(forTag:) 

Type Method

# data(forTag:)

Encodes a specified tag using BER-TLV tag encoding rules.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func data(forTag tag: TKTLVTag) -> Data
```

## Parameters 

`tag`  

The tag value to encode.

## Return Value

A data object that encodes a tag value using BER-TLV encoding.

