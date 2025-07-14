

- UIKit
- UIViewController
-  childViewControllerForPointerLock 

Instance Property

# childViewControllerForPointerLock

A child view controller to query for the pointer lock preference.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var childViewControllerForPointerLock: UIViewController? { get }
```

## Discussion

Call setNeedsUpdateOfPrefersPointerLocked() if the child view controller that the system needs to query for the pointer lock preference changes.

## See Also

### Managing pointer lock state

var prefersPointerLocked: Bool

A Boolean value that indicates whether the view controller prefers to lock the pointer to a specific scene.

func setNeedsUpdateOfPrefersPointerLocked()

Indicates that the view controller changed the pointer lock preference.

