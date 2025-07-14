

- ARKit
- ARCoachingOverlayViewDelegate
-  coachingOverlayViewDidRequestSessionReset(\_:) 

Instance Method

# coachingOverlayViewDidRequestSessionReset(\_:)

Tells you when the user taps the coaching overlay view’s Start Over button while the session is relocalizing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func coachingOverlayViewDidRequestSessionReset(_ coachingOverlayView: ARCoachingOverlayView)
```

## Discussion

Implement this function to do the actions your app requires to restart the AR experience. For example, you might hide custom relocalization UI, deallocate resources, or restore virtual content to a starting location.

If you don’t implement this function, the coaching overlay resets the session for you––equivalent to calling run(_:options:) with the resetTracking option––when the user taps Start Over.

