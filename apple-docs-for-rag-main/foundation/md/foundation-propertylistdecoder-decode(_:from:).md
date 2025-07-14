

- Foundation
- PropertyListDecoder
-  decode(\_:from:) 

Instance Method

# decode(\_:from:)

Returns a value of the specified type by decoding a property list using the default property list format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decode(
    _ type: T.Type,
    from data: Data
) throws -> T where T : Decodable
```

## Parameters 

`type`  

The type of the value to decode from the supplied property list.

`data`  

The property list to decode.

## Discussion

If the data is not a valid property list, this method throws the DecodingError.dataCorrupted(_:) error. If a value within the property list fails to decode, this method throws the corresponding error.

## See Also

### Decoding

init()

Creates a new, reusable property list decoder.

