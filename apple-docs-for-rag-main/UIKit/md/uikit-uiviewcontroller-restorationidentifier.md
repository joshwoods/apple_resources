

- UIKit
- UIViewController
-  restorationIdentifier 

Instance Property

# restorationIdentifier

The identifier that determines whether the view controller supports state restoration.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var restorationIdentifier: String? { get set }
```

## Mentioned in 

About the UI preservation process

About the UI restoration process

## Discussion

This property indicates whether the view controller and its contents should be preserved and is used to identify the view controller during the restoration process. The value of this property is `nil` by default, which indicates that the view controller should not be saved. Assigning a string object to the property lets the system know that the view controller should be saved. In addition, the contents of the string are your way to identify the purpose of the view controller.

During subsequent launches, UIKit asks your app for help in recreating the view controllers that were installed the last time your app ran. When it asks for a specific view controller, UIKit provides your app with this restoration identifier and the restoration identifiers of any parent view controllers in the view controller hierarchy. Your app must use this information to create or locate the appropriate view controller object.

Important

Simply setting the value of this property is not enough to ensure that the view controller is preserved and restored. All parent view controllers must also have a restoration identifier. For more information about the preservation and restoration process, see View Controller Programming Guide for iOS.

## See Also

### Managing state restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

var restorationClass: (any UIViewControllerRestoration.Type)?

The class responsible for recreating this view controller when restoring the app’s state.

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the view controller.

func decodeRestorableState(with: NSCoder)

Decodes and restores state-related information for the view controller.

func applicationFinishedRestoringState()

Called on restored view controllers after other object decoding is complete.

