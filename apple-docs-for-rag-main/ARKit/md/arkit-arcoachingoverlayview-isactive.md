

- ARKit
- ARCoachingOverlayView
-  isActive 

Instance Property

# isActive

A flag that indicates whether coaching is in progress.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var isActive: Bool { get }
```

## Discussion

If activatesAutomatically is enabled, this flag tells you whether coaching is in progress. Assign a delegate to coordinate your actions with the coaching overlay and allow coachingOverlayViewWillActivate(_:) to notify you when the coaching overlay is active.

When the coaching overlay is deactivating, isActive is false. If the `animated` property of setActive(_:animated:) is true, isActive and isHidden are false while the coaching overlay is fading out. When the coaching overlay is deactivated without animation, or when the animation finishes, ARKit notifies you by calling coachingOverlayViewDidDeactivate(_:).

## See Also

### Activating the View

var activatesAutomatically: Bool

A flag that indicates whether the coaching view activates automatically, depending on the current session state.

func setActive(Bool, animated: Bool)

Controls whether coaching is in progress.

