

- TVMLKit
- TVApplicationControllerDelegate
-  appController(\_:didFail:) Deprecated

Instance Method

# appController(\_:didFail:)

Tell the delegate the app controller failed due to an error.

tvOS 9.0–18.0Deprecated

``` source
optional func appController(
    _ appController: TVApplicationController,
    didFail error: any Error
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`appController`  

The TVApplicationController object that has failed.

`error`  

An NSError object describing why the app controller failed.

## See Also

### Managing the App Controller

func appController(TVApplicationController, didFinishLaunching: [String : Any]?)

Tells the delegate the app controller has finished launching.

Deprecated

func appController(TVApplicationController, didStop: [String : Any]?)

Tells the delegate the app has stopped for any reason.

Deprecated

func appController(TVApplicationController, evaluateAppJavaScriptIn: JSContext)

Tells the delegate to add JavaScript classes and objects.

Deprecated

func player(for: TVApplicationController) -> TVPlayer?

Asks the delegate for a custom player object for a particular player bridge.

Deprecated

