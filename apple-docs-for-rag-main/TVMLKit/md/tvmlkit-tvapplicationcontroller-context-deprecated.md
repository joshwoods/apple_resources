

- TVMLKit
- TVApplicationController
-  context Deprecated

Instance Property

# context

The launch information for the application controller.

tvOS 9.0–18.0Deprecated

``` source
var context: TVApplicationControllerContext { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The launch information contains the JavaScript application URL, storageIdentifier, and launchOptions. The URL can point to a local or remote resource. `launchOptions` can be constructed and forwarded from launch options keys that are part of UIApplication. See Launch Options Keys.

## See Also

### Examining App Controller Properties

var navigationController: UINavigationController

The navigation controller that is bridged from JavaScript to tvOS.

Deprecated

var window: UIWindow?

A reference to the window supplied when the app controller was initialized.

Deprecated

