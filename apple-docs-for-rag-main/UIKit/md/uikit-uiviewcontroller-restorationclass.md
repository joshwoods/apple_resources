

- UIKit
- UIViewController
-  restorationClass 

Instance Property

# restorationClass

The class responsible for recreating this view controller when restoring the app’s state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var restorationClass: (any UIViewControllerRestoration.Type)? { get set }
```

## Mentioned in 

About the UI restoration process

## Discussion

If a view controller has an associated restoration class, the viewController(withRestorationIdentifierPath:coder:) method of that class is called during state restoration. That method is responsible for returning the view controller object that matches the indicated view controller. If you do not specify a restoration class for your view controller, the state restoration engine asks your app delegate to provide the view controller object instead.

The restoration class must conform to the UIViewControllerRestoration protocol.

## See Also

### Managing state restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

var restorationIdentifier: String?

The identifier that determines whether the view controller supports state restoration.

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the view controller.

func decodeRestorableState(with: NSCoder)

Decodes and restores state-related information for the view controller.

func applicationFinishedRestoringState()

Called on restored view controllers after other object decoding is complete.

