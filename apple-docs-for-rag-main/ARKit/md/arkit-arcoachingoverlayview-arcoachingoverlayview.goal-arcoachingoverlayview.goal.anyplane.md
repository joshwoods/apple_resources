

- ARKit
- ARCoachingOverlayView
- ARCoachingOverlayView.Goal
-  ARCoachingOverlayView.Goal.anyPlane 

Case

# ARCoachingOverlayView.Goal.anyPlane

A goal that specifies your app requires a plane of any type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
case anyPlane
```

## Discussion

When you use this goal, coaching overlay won’t hide until the user has moved their device in a way that facilitates ARKit finding at least one surface. For the available surface types, see ARPlaneClassification.

## See Also

### Defining a Goal

case horizontalPlane

A goal that specifies your app requires a horizontal plane.

case tracking

A goal that specifies your app requires basic world tracking.

case verticalPlane

A goal that specifies your app requires a vertical plane.

case geoTracking

A goal that specifies your app requires a precise geographic location.

