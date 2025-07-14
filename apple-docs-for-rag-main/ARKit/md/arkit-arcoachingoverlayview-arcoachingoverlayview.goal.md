

- ARKit
- ARCoachingOverlayView
-  ARCoachingOverlayView.Goal 

Enumeration

# ARCoachingOverlayView.Goal

The options that specify your app’s tracking requirements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
enum Goal
```

## Overview

This property contains the available options when you set a coaching overlay’s goal. The coaching overlay adjusts its messaging to the user based on the value.

## Topics

### Defining a Goal

case anyPlane

A goal that specifies your app requires a plane of any type.

case horizontalPlane

A goal that specifies your app requires a horizontal plane.

case tracking

A goal that specifies your app requires basic world tracking.

case verticalPlane

A goal that specifies your app requires a vertical plane.

case geoTracking

A goal that specifies your app requires a precise geographic location.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Defining a Goal

var goal: ARCoachingOverlayView.Goal

A field that indicates your app’s tracking requirements.

