

- UIKit
- UIViewController
-  setNeedsUpdateOfPrefersPointerLocked() 

Instance Method

# setNeedsUpdateOfPrefersPointerLocked()

Indicates that the view controller changed the pointer lock preference.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
func setNeedsUpdateOfPrefersPointerLocked()
```

## See Also

### Managing pointer lock state

var prefersPointerLocked: Bool

A Boolean value that indicates whether the view controller prefers to lock the pointer to a specific scene.

var childViewControllerForPointerLock: UIViewController?

A child view controller to query for the pointer lock preference.

