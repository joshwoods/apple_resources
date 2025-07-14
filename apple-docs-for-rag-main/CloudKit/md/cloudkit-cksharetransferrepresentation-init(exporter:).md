

- CloudKit
- CKShareTransferRepresentation
-  init(exporter:) 

Initializer

# init(exporter:)

Creates and initializes a transfer representation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS

``` source
init(exporter: @escaping (Item) throws -> CKShareTransferRepresentation.ExportedShare)
```

## Parameters 

`exporter`  

A closure that provides a CKShareTransferRepresentation.ExportedShare representation of the specified `Item`.

## Return Value

A CKShareTransferRepresentation.ExportedShare.

