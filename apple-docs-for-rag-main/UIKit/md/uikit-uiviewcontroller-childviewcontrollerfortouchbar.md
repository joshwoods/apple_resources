

- UIKit
- UIViewController
-  childViewControllerForTouchBar 

Instance Property

# childViewControllerForTouchBar

The child view controller that the system uses to display content in the Touch Bar.

Mac Catalyst 13.0+

``` source
@MainActor
var childViewControllerForTouchBar: UIViewController? { get }
```

## Discussion

Override this property to have the system use the touchBar object from a child view controller instead of the current view controller. If childViewControllerForTouchBar is `nil`, the system uses the current view controller’s touchBar object.

The default value is `nil`.

## See Also

### Managing the Touch Bar

func setNeedsTouchBarUpdate()

Tells the system to update the Touch Bar.

