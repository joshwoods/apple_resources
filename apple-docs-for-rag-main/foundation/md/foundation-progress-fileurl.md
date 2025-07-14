

- Foundation
- Progress
-  fileURL 

Instance Property

# fileURL

A URL that represents the file for the current progress object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var fileURL: URL? { get set }
```

## Discussion

Set this value for a progress that you publish() to subscribers that register for updates using addSubscriber(forFileURL:withPublishingHandler:).

If present, Progress presents additional information in its localized description by setting a value in the `userInfo` dictionary.

## See Also

### Inspecting File Operation Progress Information

var fileOperationKind: Progress.FileOperationKind?

The kind of file operation for the progress object.

var fileTotalCount: Int?

The total number of files for a file progress object.

var fileCompletedCount: Int?

The number of completed files for a file progress object.

struct FileOperationKind

The kind of file operation.

