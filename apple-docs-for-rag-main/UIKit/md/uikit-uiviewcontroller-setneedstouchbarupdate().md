

- UIKit
- UIViewController
-  setNeedsTouchBarUpdate() 

Instance Method

# setNeedsTouchBarUpdate()

Tells the system to update the Touch Bar.

Mac Catalyst 13.0+

``` source
@MainActor
func setNeedsTouchBarUpdate()
```

## Discussion

Call this method when the value from childViewControllerForTouchBar changes.

## See Also

### Managing the Touch Bar

var childViewControllerForTouchBar: UIViewController?

The child view controller that the system uses to display content in the Touch Bar.

