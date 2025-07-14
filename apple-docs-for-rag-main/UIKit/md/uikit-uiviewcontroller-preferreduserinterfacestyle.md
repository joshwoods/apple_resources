

- UIKit
- UIViewController
-  preferredUserInterfaceStyle 

Instance Property

# preferredUserInterfaceStyle

The preferred interface style for this view controller.

tvOS 11.0+

``` source
@MainActor
var preferredUserInterfaceStyle: UIUserInterfaceStyle { get }
```

## Discussion

Use this property to apply a specific appearance in your tvOS app. The default value of this property is UIUserInterfaceStyle.unspecified, which causes your view controller to follow the system’s current style. You can override this property to force the view controller to adopt a specific style.

## See Also

### Adjusting the interface style

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The user interface style adopted by the view controller and all of its children.

var childViewControllerForUserInterfaceStyle: UIViewController?

The child view controller that supports the preferred user interface style.

func setNeedsUserInterfaceAppearanceUpdate()

Notifies the view controller that a change occurred that might affect the preferred interface style.

enum UIUserInterfaceStyle

Constants that indicate the interface style for the app.

