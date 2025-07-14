

- UIKit
- UIVideoEditorController
-  videoPath 

Instance Property

# videoPath

The filesystem path to the movie to be loaded by the video editor.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var videoPath: String { get set }
```

## See Also

### Configuring the editor

var videoMaximumDuration: TimeInterval

The maximum duration, in seconds, permitted for trimmed movies saved by the video editor.

var videoQuality: UIImagePickerController.QualityType

The video quality to use when saving a trimmed movie.

