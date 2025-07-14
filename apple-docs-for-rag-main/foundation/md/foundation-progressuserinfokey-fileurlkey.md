

- Foundation
- ProgressUserInfoKey
-  fileURLKey 

Type Property

# fileURLKey

A key with a corresponding value that represents the file URL of a file operation for the progress object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let fileURLKey: ProgressUserInfoKey
```

## Discussion

If present, Progress presents additional information in its localized description.

## See Also

### Using File Operation Keys

static let fileAnimationImageKey: ProgressUserInfoKey

A key with a corresponding value that is an image, typically an icon to represent the file.

static let fileAnimationImageOriginalRectKey: ProgressUserInfoKey

A key with a corresponding value that indicates the starting location of the image onscreen.

static let fileCompletedCountKey: ProgressUserInfoKey

A key with a corresponding value that represents the number of completed files.

static let fileIconKey: ProgressUserInfoKey

A key with a corresponding value that must be an image, typically an icon to represent the file.

static let fileOperationKindKey: ProgressUserInfoKey

A key with a corresponding value that indicates the kind of file operation a progress object represents.

static let fileTotalCountKey: ProgressUserInfoKey

A key with a corresponding value that represents the total number of files within a file operation.

