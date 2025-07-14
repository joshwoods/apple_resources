

- ARKit
- ARCoachingOverlayViewDelegate
-  coachingOverlayViewWillActivate(\_:) 

Instance Method

# coachingOverlayViewWillActivate(\_:)

Tells you when the coaching overlay view activates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func coachingOverlayViewWillActivate(_ coachingOverlayView: ARCoachingOverlayView)
```

## Discussion

Override this function to hide your app’s UI while the coaching overlay is active.

## See Also

### Enabling Coaching

func coachingOverlayViewDidDeactivate(ARCoachingOverlayView)

Tells you when the coaching experience is completely deactivated.

