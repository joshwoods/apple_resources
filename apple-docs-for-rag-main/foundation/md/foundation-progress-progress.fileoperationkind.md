

- Foundation
- Progress
-  Progress.FileOperationKind 

Structure

# Progress.FileOperationKind

The kind of file operation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct FileOperationKind
```

## Discussion

When tracking file operations with the progress kind set to file, provide a value for the fileOperationKindKey in the user info dictionary.

To specify the kind of file operation, provide one of the following values:

- copying

- decompressingAfterDownloading

- downloading

- uploading

- receiving

## Topics

### Creating Kinds of File Operation

init(String)

Creates a new kind of file operation using the specified string.

init(rawValue: String)

### Recognizing Kinds of File Operations

static let copying: Progress.FileOperationKind

The progress is tracking the copying of a file from source to destination.

static let decompressingAfterDownloading: Progress.FileOperationKind

The progress is tracking file decompression after a download.

static let downloading: Progress.FileOperationKind

The progress is tracking a file download operation.

static let uploading: Progress.FileOperationKind

The progress is tracking a file upload operation.

static let receiving: Progress.FileOperationKind

The progress is tracking the receipt of a file from another source.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting File Operation Progress Information

var fileOperationKind: Progress.FileOperationKind?

The kind of file operation for the progress object.

var fileURL: URL?

A URL that represents the file for the current progress object.

var fileTotalCount: Int?

The total number of files for a file progress object.

var fileCompletedCount: Int?

The number of completed files for a file progress object.

