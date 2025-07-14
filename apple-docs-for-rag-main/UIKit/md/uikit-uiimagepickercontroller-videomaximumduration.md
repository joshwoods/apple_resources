

- UIKit
- UIImagePickerController
-  videoMaximumDuration 

Instance Property

# videoMaximumDuration

The maximum duration, in seconds, for a video recording.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+

``` source
@MainActor
var videoMaximumDuration: TimeInterval { get set }
```

## Discussion

The default value for this property is 10 minutes (600 seconds). When a user taps the Share button to send a movie to MMS, MobileMe, YouTube, or another destination, an appropriate duration limit and an appropriate video quality are enforced.

This property is available only if the mediaTypes property’s value array includes the `kUTTypeMovie` media type.

## See Also

### Related Documentation

class func availableMediaTypes(for: UIImagePickerController.SourceType) -> [String]?

Retrieves the available media types for the specified source type.

class func isSourceTypeAvailable(UIImagePickerController.SourceType) -> Bool

Queries whether the device supports picking media using the specified source type.

### Configuring the video capture options

var videoQuality: UIImagePickerController.QualityType

The video recording and transcoding quality.

enum QualityType

Constants that describe video quality settings for movies that are recorded with the built-in camera, or that are transcoded when they’re displayed in the image picker.

