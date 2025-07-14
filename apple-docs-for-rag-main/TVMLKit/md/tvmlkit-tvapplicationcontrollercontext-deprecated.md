

- TVMLKit
-  TVApplicationControllerContext Deprecated

Class

# TVApplicationControllerContext

Launch information provided to the TV application controller.

tvOS 9.0–18.0Deprecated

``` source
class TVApplicationControllerContext
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Providing Launch Information

var javaScriptApplicationURL: URL

URL pointing to the controlling JavaScript file for the application.

var launchOptions: [String : Any]

Data passed to the JavaScript launch callback method.

var storageIdentifier: String?

Optional identifier for a local storage file.

var supportsPictureInPicturePlayback: Bool

A Boolean value that indicates whether your app can display content in a picture-in-picture format.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### JavaScript Environment

Implementing a Hybrid TV App with TVMLKit

Display content options with document view controllers and fetch and populate content with TVMLKit JS.

class TVApplicationController

An object that bridges the UI, navigation stack, storage, and event handling from JavaScript.

Deprecated

