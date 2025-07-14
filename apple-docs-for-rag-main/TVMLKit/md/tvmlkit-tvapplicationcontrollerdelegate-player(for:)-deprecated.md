

- TVMLKit
- TVApplicationControllerDelegate
-  player(for:) Deprecated

Instance Method

# player(for:)

Asks the delegate for a custom player object for a particular player bridge.

tvOS 12.0–18.0Deprecated

``` source
optional func player(for appController: TVApplicationController) -> TVPlayer?
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`appController`  

The TVApplicationController object that contains the player object.

## Return Value

A customizable TVPlayer object.

## See Also

### Managing the App Controller

func appController(TVApplicationController, didFail: any Error)

Tell the delegate the app controller failed due to an error.

Deprecated

func appController(TVApplicationController, didFinishLaunching: [String : Any]?)

Tells the delegate the app controller has finished launching.

Deprecated

func appController(TVApplicationController, didStop: [String : Any]?)

Tells the delegate the app has stopped for any reason.

Deprecated

func appController(TVApplicationController, evaluateAppJavaScriptIn: JSContext)

Tells the delegate to add JavaScript classes and objects.

Deprecated

