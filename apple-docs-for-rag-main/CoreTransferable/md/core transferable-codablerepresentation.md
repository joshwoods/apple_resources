

- Core Transferable
-  CodableRepresentation 

Structure

# CodableRepresentation

A transfer representation for types that participate in Swift’s protocols for encoding and decoding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct CodableRepresentation where Item : Transferable, Item : Decodable, Item : Encodable, Encoder : TopLevelEncoder, Decoder : TopLevelDecoder, Encoder.Output == Data, Decoder.Input == Data
```

## Mentioned in 

Choosing a transfer representation for a model type

## Overview

```
struct Todo: Codable, Transferable {
    var text: String
    var isDone = false

    static var transferRepresentation: some TransferRepresentation {
        CodableRepresentation(contentType: .todo)
    }
}

 extension UTType {
     static var todo: UTType { UTType(exportedAs: "com.example.todo") }
}
```

Important

If your app declares custom uniform type identifiers, include corresponding entries in the app’s `Info.plist`. For more information, see Defining file and data types for your app.

## Topics

### Creating a transfer representation

init(for: Item.Type, contentType: UTType)

Creates a transfer representation for a given type and type identifier.

init(for: Item.Type, contentType: UTType, encoder: Encoder, decoder: Decoder)

Creates a transfer representation for a given type with the encoder and decoder you supply.

### Type Aliases

typealias Body

The transfer representation for the item.

### Default Implementations

TransferRepresentation Implementations

## Relationships

### Conforms To

- Sendable
- TransferRepresentation

## See Also

### Data transfer

struct DataRepresentation

A transfer representation for types that provide their own binary data conversion.

