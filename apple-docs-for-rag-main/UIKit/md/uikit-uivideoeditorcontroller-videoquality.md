

- UIKit
- UIVideoEditorController
-  videoQuality 

Instance Property

# videoQuality

The video quality to use when saving a trimmed movie.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+

``` source
@MainActor
var videoQuality: UIImagePickerController.QualityType { get set }
```

## Discussion

The available video qualities are described in the UIImagePickerController.QualityType enumeration. The default value for this property is UIImagePickerController.QualityType.typeLow.

If a user attempts to reencode a movie to a higher quality, the movie is saved at its existing quality. Reencoding never increases movie dimensions, frame rate, or bit rate.

## See Also

### Configuring the editor

var videoMaximumDuration: TimeInterval

The maximum duration, in seconds, permitted for trimmed movies saved by the video editor.

var videoPath: String

The filesystem path to the movie to be loaded by the video editor.

