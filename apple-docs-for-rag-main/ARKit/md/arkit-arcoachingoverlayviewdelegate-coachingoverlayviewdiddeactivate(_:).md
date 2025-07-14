

- ARKit
- ARCoachingOverlayViewDelegate
-  coachingOverlayViewDidDeactivate(\_:) 

Instance Method

# coachingOverlayViewDidDeactivate(\_:)

Tells you when the coaching experience is completely deactivated.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func coachingOverlayViewDidDeactivate(_ coachingOverlayView: ARCoachingOverlayView)
```

## Discussion

Implement this function to do any custom actions your app requires to begin the AR experience. For example, when coaching is deactivated, your app might restore custom UI.

When the coaching overlay is deactivating, isActive is false. If the `animated` property of setActive(_:animated:) is true, isActive and isHidden are false while the coaching overlay is fading out. When the coaching overlay is deactivated without animation, or when the animation finishes, ARKit sends a coachingOverlayViewDidDeactivate(_:) notification.

## See Also

### Enabling Coaching

func coachingOverlayViewWillActivate(ARCoachingOverlayView)

Tells you when the coaching overlay view activates.

