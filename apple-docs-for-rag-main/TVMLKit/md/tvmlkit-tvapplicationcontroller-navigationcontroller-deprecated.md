

- TVMLKit
- TVApplicationController
-  navigationController Deprecated

Instance Property

# navigationController

The navigation controller that is bridged from JavaScript to tvOS.

tvOS 9.0–18.0Deprecated

``` source
var navigationController: UINavigationController { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The root controller in which all content is presented. Native controllers can also be pushed onto this controller, or they may be presented manually.

## See Also

### Examining App Controller Properties

var context: TVApplicationControllerContext

The launch information for the application controller.

Deprecated

var window: UIWindow?

A reference to the window supplied when the app controller was initialized.

Deprecated

