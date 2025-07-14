

- Core Transferable
- DataRepresentation
-  init(exportedContentType:exporting:) 

Initializer

# init(exportedContentType:exporting:)

Creates a representation that allows exporting an item as binary data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    exportedContentType: UTType,
    exporting: @escaping (Item) async throws -> Data
)
```

## Parameters 

`exportedContentType`  

A uniform type identifier that best describes the item.

`exporting`  

A closure that provides a data representation of the given item.

## See Also

### Creating a transfer representation

init(contentType: UTType, exporting: (Item) async throws -> Data, importing: (Data) async throws -> Item)

Creates a representation that allows transporting an item as binary data.

init(importedContentType: UTType, importing: (Data) async throws -> Item)

Creates a representation that allows importing an item as binary data.

