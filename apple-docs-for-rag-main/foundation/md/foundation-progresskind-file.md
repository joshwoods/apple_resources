

- Foundation
- ProgressKind
-  file 

Type Property

# file

The value that indicates that the progress is tracking a file operation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let file: ProgressKind
```

## Discussion

If you set this value for the progress kind, set a value in the user info dictionary for the fileOperationKindKey.

The system assumes Progress of this kind uses bytes as the unit of work. The default implementation of localizedDescription takes advantage of that to return more specific text than it does otherwise. If present, localizedDescription uses the fileTotalCountKey and fileCompletedCountKey keys in the userInfo dictionary for the overall count of files.

