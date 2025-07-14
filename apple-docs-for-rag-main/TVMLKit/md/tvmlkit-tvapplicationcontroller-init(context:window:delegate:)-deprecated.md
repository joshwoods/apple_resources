

- TVMLKit
- TVApplicationController
-  init(context:window:delegate:) Deprecated

Initializer

# init(context:window:delegate:)

Initializes and returns an app controller.

tvOS 9.0–18.0Deprecated

``` source
init(
    context: TVApplicationControllerContext,
    window: UIWindow?,
    delegate: (any TVApplicationControllerDelegate)?
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`context`  

A TVApplicationControllerContext object containing information about the JavaScript app.

`window`  

A UIWindow object that presents the application controller’s navigation controller.

`delegate`  

The app controller delegate.

## Return Value

The initialized TVApplicationController object.

## Discussion

An app controller coordinates activity between the JavaScript environments and tvOS. There are three options when presenting the application controller. If you provide a valid UIWindow object, the application controller’s navigation controller is presented immediately and managed by TVApplicationController. If no window is provided, the navigation controller can be presented and dismissed manually within the binary app. Finally, if you wish to present native view controllers alongside a TVApplicationController object, you can push additional view controllers onto navigationController.

