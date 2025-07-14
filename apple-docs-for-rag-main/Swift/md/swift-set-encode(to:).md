

- Swift
- Set
-  encode(to:) 

Instance Method

# encode(to:)

Encodes the elements of this set into the given encoder in an unkeyed container.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Element` conforms to `Encodable` and `Hashable`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

This function throws an error if any values are invalid for the given encoder’s format.

## See Also

### Encoding and Decoding

init(from: any Decoder) throws

Creates a new set by decoding from the given decoder.

