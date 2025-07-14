

- MusicKit
- ArtworkImage
-  fileExporter(isPresented:document:contentTypes:defaultFilename:onCompletion:onCancellation:) 

Instance Method

# fileExporter(isPresented:document:contentTypes:defaultFilename:onCompletion:onCancellation:)

Presents a system dialog for allowing the user to export a `ReferenceFileDocument` to a file on disk.

MusicKitSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func fileExporter(
    isPresented: Binding,
    document: D?,
    contentTypes: [UTType] = [],
    defaultFilename: String? = nil,
    onCompletion: @escaping (Result) -> Void,
    onCancellation: @escaping () -> Void = {}
) -> some View where D : ReferenceFileDocument
```

## Parameters 

`isPresented`  

A binding to whether the dialog should be shown.

`document`  

The in-memory document to export.

`contentTypes`  

The list of supported content types which can be exported. If not provided, `ReferenceFileDocument.writableContentTypes` are used.

`defaultFilename`  

If provided, the default name to use for the exported file, which will the user will have an opportunity to edit prior to the export.

`onCompletion`  

A callback that will be invoked when the operation has succeeded or failed. The `result` indicates whether the operation succeeded or failed.

`onCancellation`  

A callback that will be invoked if the user cancels the operation.

## Discussion

In order for the dialog to appear, `isPresented` must be `true`. When the operation is finished, `isPresented` will be set to `false` before `onCompletion` is called. If the user cancels the operation, `isPresented` will be set to `false` and `onCancellation` will be called.

