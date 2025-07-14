

- UIKit
- UIViewController
-  prefersPointerLocked 

Instance Property

# prefersPointerLocked

A Boolean value that indicates whether the view controller prefers to lock the pointer to a specific scene.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var prefersPointerLocked: Bool { get }
```

## Discussion

The default is false. Setting this property to true indicates the view controller’s preference to lock the pointer, although the system may not honor the request. Use isLocked to determine the current pointer lock state. For the system to consider locking the pointer:

- The scene must be full screen, not in Split View or Slide Over, with no other apps in Slide Over.

- The scene must be in the UIScene.ActivationState.foregroundActive state.

- For an app built with Mac Catalyst, the app must be in the foreground, and the window that contains the scene ordered to the front.

Note

Bringing an app built with Mac Catalyst to the foreground doesn’t immediately enable pointer lock. To enable pointer lock, the user must click in the window. To exit pointer lock, users can use Command-tab to switch to another app, or using Command-tilde.

The system continuously monitors the state and when the app no longer satisfies the requirements, it disables the pointer lock. When the lock state changes, the system posts didChangeNotification.

If you change the value of prefersPointerLocked, call setNeedsUpdateOfPrefersPointerLocked().

## See Also

### Managing pointer lock state

func setNeedsUpdateOfPrefersPointerLocked()

Indicates that the view controller changed the pointer lock preference.

var childViewControllerForPointerLock: UIViewController?

A child view controller to query for the pointer lock preference.

