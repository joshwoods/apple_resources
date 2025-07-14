

- Foundation
- ProgressUserInfoKey
-  fileIconKey 

Type Property

# fileIconKey

A key with a corresponding value that must be an image, typically an icon to represent the file.

macOS 10.9+

``` source
static let fileIconKey: ProgressUserInfoKey
```

## Discussion

If present, the Finder uses this corresponding value to show the icon of a file that a progress object is tracking.

## See Also

### Using File Operation Keys

static let fileAnimationImageKey: ProgressUserInfoKey

A key with a corresponding value that is an image, typically an icon to represent the file.

static let fileAnimationImageOriginalRectKey: ProgressUserInfoKey

A key with a corresponding value that indicates the starting location of the image onscreen.

static let fileCompletedCountKey: ProgressUserInfoKey

A key with a corresponding value that represents the number of completed files.

static let fileOperationKindKey: ProgressUserInfoKey

A key with a corresponding value that indicates the kind of file operation a progress object represents.

static let fileTotalCountKey: ProgressUserInfoKey

A key with a corresponding value that represents the total number of files within a file operation.

static let fileURLKey: ProgressUserInfoKey

A key with a corresponding value that represents the file URL of a file operation for the progress object.

