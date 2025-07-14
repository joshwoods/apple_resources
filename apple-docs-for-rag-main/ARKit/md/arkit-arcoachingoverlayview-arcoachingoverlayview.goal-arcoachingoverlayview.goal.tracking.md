

- ARKit
- ARCoachingOverlayView
- ARCoachingOverlayView.Goal
-  ARCoachingOverlayView.Goal.tracking 

Case

# ARCoachingOverlayView.Goal.tracking

A goal that specifies your app requires basic world tracking.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
case tracking
```

## Discussion

When you use this goal, coaching overlay won’t hide until the user has moved their device in a way that facilitates ARKit starting up a basic world tracking session.

## See Also

### Defining a Goal

case anyPlane

A goal that specifies your app requires a plane of any type.

case horizontalPlane

A goal that specifies your app requires a horizontal plane.

case verticalPlane

A goal that specifies your app requires a vertical plane.

case geoTracking

A goal that specifies your app requires a precise geographic location.

