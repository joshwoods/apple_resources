

- UIKit
- UINavigationController
-  init(coder:) 

Initializer

# init(coder:)

Creates a navigation controller from data in an unarchiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init?(coder aDecoder: NSCoder)
```

## See Also

### Creating a navigation controller

init(rootViewController: UIViewController)

Initializes and returns a newly created navigation controller.

init(navigationBarClass: AnyClass?, toolbarClass: AnyClass?)

Initializes and returns a newly created navigation controller that uses your custom bar subclasses.

init(nibName: String?, bundle: Bundle?)

Creates a navigation controller with the nib file in the specified bundle.

