

- FamilyControls
- FamilyActivityPicker
-  fileExporter(isPresented:document:contentType:defaultFilename:onCompletion:) 

Instance Method

# fileExporter(isPresented:document:contentType:defaultFilename:onCompletion:)

Presents a system interface for exporting a document that’s stored in a reference type, like a class, to a file on disk.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
nonisolated
func fileExporter(
    isPresented: Binding,
    document: D?,
    contentType: UTType,
    defaultFilename: String? = nil,
    onCompletion: @escaping (Result) -> Void
) -> some View where D : ReferenceFileDocument
```

## Parameters 

`isPresented`  

A binding to whether the interface should be shown.

`document`  

The in-memory document to export.

`contentType`  

The content type to use for the exported file.

`defaultFilename`  

If provided, the default name to use for the exported file, which will the user will have an opportunity to edit prior to the export.

`onCompletion`  

A callback that will be invoked when the operation has has succeeded or failed.

`result`  

A `Result` indicating whether the operation succeeded or failed.

## Discussion

In order for the interface to appear, both `isPresented` must be `true` and `document` must not be `nil`. When the operation is finished, `isPresented` will be set to `false` before `onCompletion` is called. If the user cancels the operation, `isPresented` will be set to `false` and `onCompletion` will not be called.

The `contentType` provided must be included within the document type’s `writableContentTypes`, otherwise the first valid writable content type will be used instead.

## See Also

### File Managers

func fileExporter&lt;D>(isPresented: Binding&lt;Bool>, document: D?, contentType: UTType, defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for exporting a document that’s stored in a value type, like a structure, to a file on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentType: UTType, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for exporting a collection of value type documents to files on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentType: UTType, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for exporting a collection of reference type documents to files on disk.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], allowsMultipleSelection: Bool, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import multiple files.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import an existing file.

func fileMover(isPresented: Binding&lt;Bool>, file: URL?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for allowing the user to move an existing file to a new location.

func fileMover&lt;C>(isPresented: Binding&lt;Bool>, files: C, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to move a collection of existing files to a new location.

