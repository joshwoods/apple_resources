

- UIKit
- UINavigationController
-  init(navigationBarClass:toolbarClass:) 

Initializer

# init(navigationBarClass:toolbarClass:)

Initializes and returns a newly created navigation controller that uses your custom bar subclasses.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    navigationBarClass: AnyClass?,
    toolbarClass: AnyClass?
)
```

## Parameters 

`navigationBarClass`  

Specify the custom UINavigationBar subclass you want to use, or specify `nil` to use the standard UINavigationBar class.

`toolbarClass`  

Specify the custom UIToolbar subclass you want to use, or specify `nil` to use the standard UIToolbar class.

## Return Value

The initialized navigation controller object or `nil` if there was a problem initializing the object.

## Discussion

To customize the overall appearance of a navigation bar, use UIAppearance APIs instead of this method. If you use this initialization method to create a navigation bar that uses custom bar subclasses, you are responsible for pushing and setting view controllers before presenting the navigation controller onscreen.

## See Also

### Creating a navigation controller

init(rootViewController: UIViewController)

Initializes and returns a newly created navigation controller.

init(nibName: String?, bundle: Bundle?)

Creates a navigation controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a navigation controller from data in an unarchiver.

