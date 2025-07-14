

- RealityKit
-  HasBodyTracking 

Protocol

# HasBodyTracking

An interface that enables the animation of a virtual character by tracking a real person in AR.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @preconcurrency
protocol HasBodyTracking : HasTransform
```

## Overview

Important

Body tracking requires a compatible rigged model. For more information on creating a compatible model, see Rigging a Model for Motion Capture.

## Topics

### Accessing the component

var bodyTracking: BodyTrackingComponent

The body-tracking component for the body-tracked entity.

## Relationships

### Inherits From

- HasTransform

### Conforming Types

- BodyTrackedEntity

## See Also

### Body and face tracking

Creating an App for Face-Painting in AR

Combine RealityKit’s face detection with PencilKit to implement virtual face-painting.

Occluding virtual content with people

Cover your app’s virtual content with people that ARKit perceives in the camera feed.

struct BodyTrackingComponent

A component for tracking people in an AR session.

class BodyTrackedEntity

An entity used to animate a virtual character in an AR scene by tracking a real person.

