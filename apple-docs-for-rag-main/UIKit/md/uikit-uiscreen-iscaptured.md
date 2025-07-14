

- UIKit
- UIScreen
-  isCaptured 

Instance Property

# isCaptured

A Boolean value that indicates whether the system is actively cloning the screen to another destination.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+tvOS 11.0+

``` source
@MainActor
var isCaptured: Bool { get }
```

## Discussion

A value of `YES` indicates the system is actively recording, mirroring, or using AirPlay to stream the contents of the screen.

Observe this property and optionally take an appropriate action in your app to prevent the capture of your content. For example, a media app might stop any current media playback and present a dialog to the user describing the reason for the pause.

Important

The system doesn’t include video content encrypted using FairPlay Streaming (FPS) when recording, mirroring, or using AirPlay to stream the contents of the screen. However, although it blacks out FPS-encrypted video content, it includes FPS-encrypted audio content. To prevent the system from recording the audio portion, observe the `isCaptured` property and take appropriate action in your app as described above.

UIKit sends the capturedDidChangeNotification notification when the capture status of the screen changes.

## See Also

### Related Documentation

class let userDidTakeScreenshotNotification: NSNotification.Name

A notification that posts when a person takes a screenshot on the device.

### Detecting screen capture

var mirrored: UIScreen?

The screen an external display mirrors from.

