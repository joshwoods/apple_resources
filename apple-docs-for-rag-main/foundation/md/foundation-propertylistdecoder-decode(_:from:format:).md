

- Foundation
- PropertyListDecoder
-  decode(\_:from:format:) 

Instance Method

# decode(\_:from:format:)

Returns a value of the specified type by decoding a property list using the supplied format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func decode(
    _ type: T.Type,
    from data: Data,
    format: inout PropertyListDecoder.PropertyListFormat
) throws -> T where T : Decodable
```

## Discussion

If the data is not a valid property list, this method throws the DecodingError.dataCorrupted(_:) error. If a value within the property list fails to decode, this method throws the corresponding error.

## See Also

### Customizing Decoding

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize decoding by providing contextual information.

