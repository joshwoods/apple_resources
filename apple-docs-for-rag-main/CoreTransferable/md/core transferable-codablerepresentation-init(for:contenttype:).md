

- Core Transferable
- CodableRepresentation
-  init(for:contentType:) 

Initializer

# init(for:contentType:)

Creates a transfer representation for a given type and type identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    for itemType: Item.Type = Item.self,
    contentType: UTType
) where Encoder == JSONEncoder, Decoder == JSONDecoder
```

## Parameters 

`itemType`  

The concrete type of the item that’s being transferred.

`contentType`  

A uniform type identifier that best describes the item.

## Discussion

This initializer uses JSON for encoding and decoding.

## See Also

### Creating a transfer representation

init(for: Item.Type, contentType: UTType, encoder: Encoder, decoder: Decoder)

Creates a transfer representation for a given type with the encoder and decoder you supply.

