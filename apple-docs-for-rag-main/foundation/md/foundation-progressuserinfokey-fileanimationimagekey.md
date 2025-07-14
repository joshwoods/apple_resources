

- Foundation
- ProgressUserInfoKey
-  fileAnimationImageKey 

Type Property

# fileAnimationImageKey

A key with a corresponding value that is an image, typically an icon to represent the file.

macOS 10.9+

``` source
static let fileAnimationImageKey: ProgressUserInfoKey
```

## Discussion

This entry is optional, but if present, along with a value for fileAnimationImageOriginalRectKey, the Dock may show an animation. When the Dock has an item for the folder that contains the relevant file (such as the Downloads folder), the Dock uses this key to show an animation of the file flying into the Dock.

## See Also

### Using File Operation Keys

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

static let fileURLKey: ProgressUserInfoKey

A key with a corresponding value that represents the file URL of a file operation for the progress object.

