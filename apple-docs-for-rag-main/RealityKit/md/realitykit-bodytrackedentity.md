

- RealityKit
-  BodyTrackedEntity 

Class

# BodyTrackedEntity

An entity used to animate a virtual character in an AR scene by tracking a real person.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+

``` source
@MainActor @preconcurrency
class BodyTrackedEntity
```

## Mentioned in 

Loading entities from a file

## Overview

Like a ModelEntity, a BodyTrackedEntity has a ModelComponent that defines its physical appearance. Unlike a model entity, a body-tracked entity lacks the components required to participate in collisions or physics simulations. Instead, a BodyTrackingComponent drives the positioning and arrangement of the entity based on tracking information from the AR session.

For an example of how to use a body-tracked entity, see Capturing Body Motion in 3D.

## Topics

### Configuring body tracking

var bodyTracking: BodyTrackingComponent

The body-tracking component for the body-tracked entity.

### Configuring the model

var model: ModelComponent?

The model component for the entity.

var jointNames: [String]

The names of all the joints in the model entity.

var jointTransforms: [Transform]

The relative joint transforms of the model entity.

### Setting debug options

var modelDebugOptions: ModelDebugOptionsComponent?

Configures the debug visualization of this model.

### Default Implementations

HasBodyTracking Implementations

HasModel Implementations

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasBodyTracking
- HasHierarchy
- HasModel
- HasSynchronization
- HasTransform
- Hashable
- Identifiable
- RealityCoordinateSpace
- Sendable

## See Also

### Body and face tracking

Creating an App for Face-Painting in AR

Combine RealityKit’s face detection with PencilKit to implement virtual face-painting.

Occluding virtual content with people

Cover your app’s virtual content with people that ARKit perceives in the camera feed.

struct BodyTrackingComponent

A component for tracking people in an AR session.

protocol HasBodyTracking

An interface that enables the animation of a virtual character by tracking a real person in AR.

