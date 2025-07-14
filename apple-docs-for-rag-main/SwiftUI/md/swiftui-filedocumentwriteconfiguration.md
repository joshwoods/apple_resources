

- SwiftUI
-  FileDocumentWriteConfiguration 

Structure

# FileDocumentWriteConfiguration

The configuration for serializing file contents.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct FileDocumentWriteConfiguration
```

## Topics

### Writing the content

let contentType: UTType

The expected uniform type of the file contents.

let existingFile: FileWrapper?

The file wrapper containing the current document content. `nil` if the document is unsaved.

## See Also

### Reading and writing documents

struct FileDocumentReadConfiguration

The configuration for reading file contents.

