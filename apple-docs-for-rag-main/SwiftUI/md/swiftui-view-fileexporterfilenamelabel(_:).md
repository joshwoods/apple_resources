

- SwiftUI
- View
-  fileExporterFilenameLabel(\_:) 

Instance Method

# fileExporterFilenameLabel(\_:)

On macOS, configures the `fileExporter` with a text to use as a label for the file name field.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func fileExporterFilenameLabel(_ label: Text?) -> some View
```

Show all declarations

## Parameters 

`label`  

The optional text to use as the label for the file name field.

## See Also

### Exporting to file

func fileExporter(isPresented:document:contentType:defaultFilename:onCompletion:)

Presents a system interface for exporting a document that’s stored in a value type, like a structure, to a file on disk.

func fileExporter(isPresented:documents:contentType:onCompletion:)

Presents a system interface for exporting a collection of value type documents to files on disk.

func fileExporter(isPresented:document:contentTypes:defaultFilename:onCompletion:onCancellation:)

Presents a system interface for allowing the user to export a `FileDocument` to a file on disk.

func fileExporter(isPresented:documents:contentTypes:onCompletion:onCancellation:)

Presents a system dialog for allowing the user to export a collection of documents that conform to `FileDocument` to files on disk.

func fileExporter&lt;T>(isPresented: Binding&lt;Bool>, item: T?, contentTypes: [UTType], defaultFilename: String?, onCompletion: (Result&lt;URL, any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a `Transferable` item to file on disk.

func fileExporter&lt;C, T>(isPresented: Binding&lt;Bool>, items: C, contentTypes: [UTType], onCompletion: (Result&lt;[URL], any Error>) -> Void, onCancellation: () -> Void) -> some View

Presents a system interface allowing the user to export a collection of items to files on disk.

