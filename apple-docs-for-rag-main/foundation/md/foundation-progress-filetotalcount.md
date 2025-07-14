

- Foundation
- Progress
-  fileTotalCount 

Instance Property

# fileTotalCount

The total number of files for a file progress object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var fileTotalCount: Int? { get set }
```

## Discussion

If the current progress is operating on a set of files, set this property to the total number of files in the operation.

If present, Progress presents additional information in its localized description by setting a value in the `userInfo` dictionary.

## See Also

### Inspecting File Operation Progress Information

var fileOperationKind: Progress.FileOperationKind?

The kind of file operation for the progress object.

var fileURL: URL?

A URL that represents the file for the current progress object.

var fileCompletedCount: Int?

The number of completed files for a file progress object.

struct FileOperationKind

The kind of file operation.

