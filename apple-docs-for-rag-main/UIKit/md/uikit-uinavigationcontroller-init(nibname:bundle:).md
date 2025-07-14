

- UIKit
- UINavigationController
-  init(nibName:bundle:) 

Initializer

# init(nibName:bundle:)

Creates a navigation controller with the nib file in the specified bundle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    nibName nibNameOrNil: String?,
    bundle nibBundleOrNil: Bundle?
)
```

## See Also

### Creating a navigation controller

init(rootViewController: UIViewController)

Initializes and returns a newly created navigation controller.

init(navigationBarClass: AnyClass?, toolbarClass: AnyClass?)

Initializes and returns a newly created navigation controller that uses your custom bar subclasses.

init?(coder: NSCoder)

Creates a navigation controller from data in an unarchiver.

