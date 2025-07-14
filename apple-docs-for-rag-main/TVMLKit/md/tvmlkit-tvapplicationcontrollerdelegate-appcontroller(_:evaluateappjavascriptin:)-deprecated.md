

- TVMLKit
- TVApplicationControllerDelegate
-  appController(\_:evaluateAppJavaScriptIn:) Deprecated

Instance Method

# appController(\_:evaluateAppJavaScriptIn:)

Tells the delegate to add JavaScript classes and objects.

tvOS 9.0–18.0Deprecated

``` source
optional func appController(
    _ appController: TVApplicationController,
    evaluateAppJavaScriptIn jsContext: JSContext
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`appController`  

The TVApplicationController object that is evaluating the JavaScript context.

`jsContext`  

The JSContext object being evaluated.

## Discussion

This method serves as a callback function, giving the delegate the ability to add JavaScript classes and objects through the setObject:forKeyedSubscript: method using the `jsContext` parameter. This method is called before the JavaScript is parsed into the execution context and is called on the JavaScript execution thread, not the main thread. Any object exposed to JSContext must not be retained on any other thread.

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

func player(for: TVApplicationController) -> TVPlayer?

Asks the delegate for a custom player object for a particular player bridge.

Deprecated

