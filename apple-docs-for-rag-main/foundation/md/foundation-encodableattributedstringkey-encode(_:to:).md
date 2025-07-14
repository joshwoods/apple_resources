

- Foundation
- EncodableAttributedStringKey
-  encode(\_:to:) 

Type Method

# encode(\_:to:)

Encodes a value to the provided encoder.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func encode(
    _ value: Self.Value,
    to encoder: any Encoder
) throws
```

**Required** Default implementations provided.

## Parameters 

`value`  

The value to encode.

`encoder`  

The encoder to write data to.

## Discussion

This method throws an error if writing to the encoder fails.

## Default Implementations

### EncodableAttributedStringKey Implementations

static func encode(Self.Value, to: any Encoder) throws

static func encode(Self.Value, to: any Encoder) throws

Encodes an Objective-C value to the provided encoder, using a default implementation.

