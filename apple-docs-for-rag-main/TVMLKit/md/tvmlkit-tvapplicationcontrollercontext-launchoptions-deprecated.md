

- TVMLKit
- TVApplicationControllerContext
-  launchOptions Deprecated

Instance Property

# launchOptions

Data passed to the JavaScript launch callback method.

tvOS 9.0–18.0Deprecated

``` source
var launchOptions: [String : Any] { get set }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The system will pass this data to the JavaScript onLaunch method. The values contained in this property must be serializable. You must include url and sourceApplication in the launch options if the JavaScript implements the openURL(_:) method.

## See Also

### Providing Launch Information

var javaScriptApplicationURL: URL

URL pointing to the controlling JavaScript file for the application.

Deprecated

var storageIdentifier: String?

Optional identifier for a local storage file.

Deprecated

var supportsPictureInPicturePlayback: Bool

A Boolean value that indicates whether your app can display content in a picture-in-picture format.

Deprecated

