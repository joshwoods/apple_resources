

- CryptoTokenKit
- TKTLVRecord
-  init(from:) 

Initializer

# init(from:)

Creates and returns a TLV record from by parsing the specified data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init?(from data: Data)
```

## Parameters 

`data`  

A data object containing the serialized representation of a TLV record.

## Return Value

A TLV record, or `nil` if `data` does not specify a valid record.

## See Also

### Creating Records

class func sequenceOfRecords(from: Data) -> [TKTLVRecord]?

Creates and returns an array of TLV records from the specified data.

