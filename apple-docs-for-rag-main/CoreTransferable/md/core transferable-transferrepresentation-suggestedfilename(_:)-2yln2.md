

- Core Transferable
- TransferRepresentation
-  suggestedFileName(\_:) 

Instance Method

# suggestedFileName(\_:)

Provides a filename to use if the receiver chooses to write the item to disk.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func suggestedFileName(_ fileName: String) -> some TransferRepresentation
```

## Parameters 

`fileName`  

The suggested filename including the filename extension. If several suggested file names are specified on an item, only the last one will be used.

## Discussion

Any transfer representation can be written to disk.

```
 extension ImageDocumentLayer: Transferable {
     static var transferRepresentation: some TransferRepresentation {
         DataRepresentation(contentType: .layer) { layer in
             layer.data()
             } importing: { data in
                 try ImageDocumentLayer(data: data)
             }
             .suggestedFileName("Layer.exampleLayer")
         DataRepresentation(exportedContentType: .png) { layer in
             layer.pngData()
         }
         .suggestedFileName("Layer.png")
     }
 }
```

The .exampleLayer filename extension above should match the extension for the `layer` content type, which you declare in your app’s `Info.plist` file.

