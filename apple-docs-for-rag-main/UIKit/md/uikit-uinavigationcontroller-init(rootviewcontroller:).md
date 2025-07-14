

- UIKit
- UINavigationController
-  init(rootViewController:) 

Initializer

# init(rootViewController:)

Initializes and returns a newly created navigation controller.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(rootViewController: UIViewController)
```

## Parameters 

`rootViewController`  

The view controller that resides at the bottom of the navigation stack. This object cannot be an instance of the UITabBarController class.

## Return Value

The initialized navigation controller object or `nil` if there was a problem initializing the object.

## Discussion

This is a convenience method for initializing the receiver and pushing a root view controller onto the navigation stack. Every navigation stack must have at least one view controller to act as the root.

## See Also

### Creating a navigation controller

init(navigationBarClass: AnyClass?, toolbarClass: AnyClass?)

Initializes and returns a newly created navigation controller that uses your custom bar subclasses.

init(nibName: String?, bundle: Bundle?)

Creates a navigation controller with the nib file in the specified bundle.

init?(coder: NSCoder)

Creates a navigation controller from data in an unarchiver.

