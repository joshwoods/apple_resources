

- Core Transferable
-  DataRepresentation 

Structure

# DataRepresentation

A transfer representation for types that provide their own binary data conversion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct DataRepresentation where Item : Transferable
```

## Mentioned in 

Choosing a transfer representation for a model type

## Overview

Use this transfer representation if your model is stored in memory. For example, a drawing app might have a notion of a *layer* that can be converted to and from a custom binary data format and also converted to the PNG image type:

```
struct ImageDocumentLayer {
    init(data: Data) throws
    func data() -> Data
    func pngData() -> Data
}
```

You can provide multiple transfer representations for a model type, even if the transfer representation types are the same. The following shows the `ImageDocumentLayer` structure conforming to `Transferable` with two DataRepresentation instances composed together:

```
extension ImageDocumentLayer: Transferable {
    static var transferRepresentation: some TransferRepresentation {
        DataRepresentation(contentType: .layer) { layer in
                layer.data()
            } importing: { data in
                try ImageDocumentLayer(data: data)
            }
        DataRepresentation(exportedContentType: .png) { layer in
            layer.pngData()
        }
    }
}
```

The example drawing app’s custom transfer representation comes first so that apps that know about the custom transfer representation can use it. The second transfer representation offers export compatibility with other apps that work with PNG images.

Tip

If a type conforms to `Codable`, CodableRepresentation might be a more convenient choice than DataRepresentation.

## Topics

### Creating a transfer representation

init(contentType: UTType, exporting: (Item) async throws -> Data, importing: (Data) async throws -> Item)

Creates a representation that allows transporting an item as binary data.

init(importedContentType: UTType, importing: (Data) async throws -> Item)

Creates a representation that allows importing an item as binary data.

init(exportedContentType: UTType, exporting: (Item) async throws -> Data)

Creates a representation that allows exporting an item as binary data.

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

struct CodableRepresentation

A transfer representation for types that participate in Swift’s protocols for encoding and decoding.

