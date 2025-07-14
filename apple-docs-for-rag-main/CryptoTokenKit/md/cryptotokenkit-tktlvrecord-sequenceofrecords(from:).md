

- CryptoTokenKit
- TKTLVRecord
-  sequenceOfRecords(from:) 

Type Method

# sequenceOfRecords(from:)

Creates and returns an array of TLV records from the specified data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class func sequenceOfRecords(from data: Data) -> [TKTLVRecord]?
```

## Parameters 

`data`  

A data object containing the serialized representation of zero or more TLV records.

## Return Value

A sequence of TLV records, or `nil` if `data` does not specify a sequence of valid records.

## See Also

### Creating Records

convenience init?(from: Data)

Creates and returns a TLV record from by parsing the specified data.

