

- UIKit
- UIViewController
-  childViewControllerForUserInterfaceStyle 

Instance Property

# childViewControllerForUserInterfaceStyle

The child view controller that supports the preferred user interface style.

tvOS 11.0+

``` source
@MainActor
var childViewControllerForUserInterfaceStyle: UIViewController? { get }
```

## Discussion

The default value of this property is `nil`. A container view controller can override this property and return the child view controller that supports the currently preferred user interface style, as determined by the preferredUserInterfaceStyle property.

## See Also

### Adjusting the interface style

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The user interface style adopted by the view controller and all of its children.

var preferredUserInterfaceStyle: UIUserInterfaceStyle

The preferred interface style for this view controller.

func setNeedsUserInterfaceAppearanceUpdate()

Notifies the view controller that a change occurred that might affect the preferred interface style.

enum UIUserInterfaceStyle

Constants that indicate the interface style for the app.

