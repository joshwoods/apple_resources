

- SwiftUI
- View
-  fileExporter(isPresented:document:contentTypes:defaultFilename:onCompletion:onCancellation:) 

Instance Method

# fileExporter(isPresented:document:contentTypes:defaultFilename:onCompletion:onCancellation:)

Presents a system interface for allowing the user to export a `FileDocument` to a file on disk.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func fileExporter(
    isPresented: Binding,
    document: D?,
    contentTypes: [UTType] = [],
    defaultFilename: String? = nil,
    onCompletion: @escaping (Result) -> Void,
    onCancellation: @escaping () -> Void = {}
) -> some View where D : FileDocument
```

Show all declarations

## Parameters 

`isPresented`  

A binding to whether the interface should be shown.

`document`  

The in-memory document to export.

`contentTypes`  

The list of supported content types which can be exported. If not provided, `FileDocument.writableContentTypes` are used.

`defaultFilename`  

If provided, the default name to use for the exported file, which will the user will have an opportunity to edit prior to the export.

`onCompletion`  

A callback that will be invoked when the operation has succeeded or failed. The `result` indicates whether the operation succeeded or failed.

`onCancellation`  

A callback that will be invoked if the user cancels the operation.

## Discussion

In order for the interface to appear, `isPresented` must be `true`. When the operation is finished, `isPresented` will be set to `false` before `onCompletion` is called. If the user cancels the operation, `isPresented` will be set to `false` and `onCancellation` will be called.

## See Also

### Exporting to file

func fileExporter(isPresented:document:contentType:defaultFilename:onCompletion:)

Presents a system interface for exporting a document that’s stored in a value type, like a structure, to a file on disk.

func fileExporter(isPresented:documents:contentType:onCompletion:)

Presents a system interface for exporting a collection of value type documents to files on disk.

func fileExporter(isPresented:documents:contentTypes:onCompletion:onCancellation:)

Presents a system dialog for allowing the user to export a collection of documents that conform to `FileDocument` to files on disk.

func fileExporter&lt;T>(isPresented: Binding&lt;Bool>, item: T?, contentTypes: [UTType], defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a `Transferable` item to file on disk.

func fileExporter&lt;C, T>(isPresented: Binding&lt;Bool>, items: C, contentTypes: [UTType], onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a collection of items to files on disk.

func fileExporterFilenameLabel(_:)

On macOS, configures the `fileExporter` with a text to use as a label for the file name field.

