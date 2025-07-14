

- UIKit
- UIViewController
-  setNeedsUserInterfaceAppearanceUpdate() 

Instance Method

# setNeedsUserInterfaceAppearanceUpdate()

Notifies the view controller that a change occurred that might affect the preferred interface style.

tvOS 11.0+

``` source
@MainActor
func setNeedsUserInterfaceAppearanceUpdate()
```

## Discussion

UIKit calls this method to let the view controller know when system-level interface style changes occur. You can also call it to let UIKit know when you change your view controller in a way that affects the preferred user interface style.

## See Also

### Adjusting the interface style

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The user interface style adopted by the view controller and all of its children.

var preferredUserInterfaceStyle: UIUserInterfaceStyle

The preferred interface style for this view controller.

var childViewControllerForUserInterfaceStyle: UIViewController?

The child view controller that supports the preferred user interface style.

enum UIUserInterfaceStyle

Constants that indicate the interface style for the app.

