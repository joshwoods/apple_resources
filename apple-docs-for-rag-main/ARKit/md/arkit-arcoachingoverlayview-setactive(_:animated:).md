

- ARKit
- ARCoachingOverlayView
-  setActive(\_:animated:) 

Instance Method

# setActive(\_:animated:)

Controls whether coaching is in progress.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
func setActive(
    _ active: Bool,
    animated: Bool
)
```

## Parameters 

`active`  

A flag you set to indicate whether the coaching overlay should activate or deactivate.

`animated`  

A flag that when true, fades the coaching overlay in or out. When you pass a value of false, the coaching overlay shows or hides instantly.

## Discussion

If the `animated` property of setActive(_:animated:) is true, isActive and isHidden are false while the coaching overlay is fading out. When the coaching overlay is deactivated without animation, or when the animation finishes, ARKit notifies you by calling coachingOverlayViewDidDeactivate(_:).

## See Also

### Activating the View

var activatesAutomatically: Bool

A flag that indicates whether the coaching view activates automatically, depending on the current session state.

var isActive: Bool

A flag that indicates whether coaching is in progress.

