

- TVMLKit
- TVApplicationController
-  delegate Deprecated

Instance Property

# delegate

The delegate of the app controller object.

tvOS 9.0–18.0Deprecated

``` source
weak var delegate: (any TVApplicationControllerDelegate)? { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The delegate provides methods for observing and managing different `TVApplicationController` object states. TVApplicationControllerDelegate provides callbacks during the launch of the JavaScript application.

## See Also

### Getting the Delegate

protocol TVApplicationControllerDelegate

A protocol used to observe and manage the different states of an application controller.

Deprecated

