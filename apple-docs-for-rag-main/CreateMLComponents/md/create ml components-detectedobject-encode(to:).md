

- Create ML Components
- DetectedObject
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func encode(to encoder: any Encoder) throws
```

Available when `Label` conforms to `Comparable`, `Encodable`, and `Hashable`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

If the value fails to encode anything, `encoder` will encode an empty keyed container in its place.

This function throws an error if any values are invalid for the given encoder’s format.

