

- TVMLKit
- TVApplicationControllerContext
-  supportsPictureInPicturePlayback Deprecated

Instance Property

# supportsPictureInPicturePlayback

A Boolean value that indicates whether your app can display content in a picture-in-picture format.

tvOS 9.0–18.0Deprecated

``` source
var supportsPictureInPicturePlayback: Bool { get set }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

When this property is set to true, the system allows the user to continue watching your app’s video content while using other apps. If you customize playback with AVPlayerViewController, set the controller’s delegate property to an object that implements the AVPlayerViewControllerDelegate protocol and the system will notify that object about picture-in-picture playback events.

The default value is true.

## See Also

### Providing Launch Information

var javaScriptApplicationURL: URL

URL pointing to the controlling JavaScript file for the application.

Deprecated

var launchOptions: [String : Any]

Data passed to the JavaScript launch callback method.

Deprecated

var storageIdentifier: String?

Optional identifier for a local storage file.

Deprecated

