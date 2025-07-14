

- FamilyControls
- FamilyActivityPicker
-  fileMover(isPresented:file:onCompletion:) 

Instance Method

# fileMover(isPresented:file:onCompletion:)

Presents a system interface for allowing the user to move an existing file to a new location.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
nonisolated
func fileMover(
    isPresented: Binding,
    file: URL?,
    onCompletion: @escaping (Result) -> Void
) -> some View
```

## Parameters 

`isPresented`  

A binding to whether the interface should be shown.

`file`  

The `URL` of the file to be moved.

`onCompletion`  

A callback that will be invoked when the operation has has succeeded or failed. To access the received URLs, call `startAccessingSecurityScopedResource`. When the access is no longer required, call `stopAccessingSecurityScopedResource`.

`result`  

A `Result` indicating whether the operation succeeded or failed.

## Discussion

Note

This interface provides security-scoped URLs. Call the `startAccessingSecurityScopedResource` method to access or bookmark the URLs, and the `stopAccessingSecurityScopedResource` method to release the access.

In order for the interface to appear, both `isPresented` must be `true` and `file` must not be `nil`. When the operation is finished, `isPresented` will be set to `false` before `onCompletion` is called. If the user cancels the operation, `isPresented` will be set to `false` and `onCompletion` will not be called.

## See Also

### File Managers

func fileExporter&lt;D>(isPresented: Binding&lt;Bool>, document: D?, contentType: UTType, defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for exporting a document that’s stored in a value type, like a structure, to a file on disk.

func fileExporter&lt;D>(isPresented: Binding&lt;Bool>, document: D?, contentType: UTType, defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for exporting a document that’s stored in a reference type, like a class, to a file on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentType: UTType, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for exporting a collection of value type documents to files on disk.

func fileExporter&lt;C>(isPresented: Binding&lt;Bool>, documents: C, contentType: UTType, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for exporting a collection of reference type documents to files on disk.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], allowsMultipleSelection: Bool, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import multiple files.

func fileImporter(isPresented: Binding&lt;Bool>, allowedContentTypes: [UTType], onCompletion: (Result&lt;URL, any Error>) -> Void) -> some View

Presents a system interface for allowing the user to import an existing file.

func fileMover&lt;C>(isPresented: Binding&lt;Bool>, files: C, onCompletion: (Result&lt;[URL], any Error>) -> Void) -> some View

Presents a system interface for allowing the user to move a collection of existing files to a new location.

