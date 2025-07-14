

- App Intents
- EntityProperty
-  encode(to:) 

Instance Method

# encode(to:)

Encodes this value into the given encoder.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
final func encode(to encoder: any Encoder) throws
```

Available when `Value` conforms to `_IntentValue`, `Decodable`, `Encodable`, and `Sendable`.

## Parameters 

`encoder`  

The encoder to write data to.

## Discussion

If the value fails to encode anything, `encoder` will encode an empty keyed container in its place.

This function throws an error if any values are invalid for the given encoder’s format.

