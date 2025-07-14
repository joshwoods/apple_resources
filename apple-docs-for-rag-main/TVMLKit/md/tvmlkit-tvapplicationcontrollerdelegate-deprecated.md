

- TVMLKit
-  TVApplicationControllerDelegate Deprecated

Protocol

# TVApplicationControllerDelegate

A protocol used to observe and manage the different states of an application controller.

tvOS 9.0–18.0Deprecated

``` source
protocol TVApplicationControllerDelegate : NSObjectProtocol
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Managing the App Controller

func appController(TVApplicationController, didFail: any Error)

Tell the delegate the app controller failed due to an error.

func appController(TVApplicationController, didFinishLaunching: [String : Any]?)

Tells the delegate the app controller has finished launching.

func appController(TVApplicationController, didStop: [String : Any]?)

Tells the delegate the app has stopped for any reason.

func appController(TVApplicationController, evaluateAppJavaScriptIn: JSContext)

Tells the delegate to add JavaScript classes and objects.

func player(for: TVApplicationController) -> TVPlayer?

Asks the delegate for a custom player object for a particular player bridge.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting the Delegate

var delegate: (any TVApplicationControllerDelegate)?

The delegate of the app controller object.

Deprecated

