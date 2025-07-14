

- UIKit
- UIViewController
-  overrideUserInterfaceStyle 

Instance Property

# overrideUserInterfaceStyle

The user interface style adopted by the view controller and all of its children.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var overrideUserInterfaceStyle: UIUserInterfaceStyle { get set }
```

## Discussion

Use this property to force the view controller to always adopt a light or dark interface style. The default value of this property is UIUserInterfaceStyle.unspecified, which causes the view controller to inherit the interface style from the system or a parent view controller. If you assign a different value, the new style applies to the view controller, its entire view hierarchy, and any embedded child view controllers.

## See Also

### Adjusting the interface style

var preferredUserInterfaceStyle: UIUserInterfaceStyle

The preferred interface style for this view controller.

var childViewControllerForUserInterfaceStyle: UIViewController?

The child view controller that supports the preferred user interface style.

func setNeedsUserInterfaceAppearanceUpdate()

Notifies the view controller that a change occurred that might affect the preferred interface style.

enum UIUserInterfaceStyle

Constants that indicate the interface style for the app.

