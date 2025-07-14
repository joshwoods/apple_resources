

- RealityKit
-  BodyTrackingComponent 

Structure

# BodyTrackingComponent

A component for tracking people in an AR session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
struct BodyTrackingComponent
```

## Overview

Body tracking requires a compatible rigged model. For more information on creating a compatible model, see Rigging a Model for Motion Capture.

For a sample app that uses body tracking, see Capturing Body Motion in 3D

## Topics

### Creating a body tracking component

init()

Creates a body-tracking component.

init(BodyTrackingComponent.Target)

Creates a body-tracking component for the given target.

### Pausing body tracking

var isPaused: Bool

A Boolean that you can set to temporarily stop applying body tracking to the model and freeze the model in its current pose.

### Selecting a body to track

var target: BodyTrackingComponent.Target

The body-tracking setting.

enum Target

Body-tracking settings for selecting a person to track.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing body tracking components

static func == (BodyTrackingComponent, BodyTrackingComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Body and face tracking

Creating an App for Face-Painting in AR

Combine RealityKit’s face detection with PencilKit to implement virtual face-painting.

Occluding virtual content with people

Cover your app’s virtual content with people that ARKit perceives in the camera feed.

class BodyTrackedEntity

An entity used to animate a virtual character in an AR scene by tracking a real person.

protocol HasBodyTracking

An interface that enables the animation of a virtual character by tracking a real person in AR.

