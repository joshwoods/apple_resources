

- TVMLKit
- TVApplicationControllerDelegate
-  appController(\_:didStop:) Deprecated

Instance Method

# appController(\_:didStop:)

Tells the delegate the app has stopped for any reason.

tvOS 9.0–18.0Deprecated

``` source
optional func appController(
    _ appController: TVApplicationController,
    didStop options: [String : Any]?
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`appController`  

The TVApplicationController object that has stopped.

`options`  

The launch options passed to the app controller.

## See Also

### Managing the App Controller

func appController(TVApplicationController, didFail: any Error)

Tell the delegate the app controller failed due to an error.

Deprecated

func appController(TVApplicationController, didFinishLaunching: [String : Any]?)

Tells the delegate the app controller has finished launching.

Deprecated

func appController(TVApplicationController, evaluateAppJavaScriptIn: JSContext)

Tells the delegate to add JavaScript classes and objects.

Deprecated

func player(for: TVApplicationController) -> TVPlayer?

Asks the delegate for a custom player object for a particular player bridge.

Deprecated

