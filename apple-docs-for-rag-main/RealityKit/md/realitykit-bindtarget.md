

- RealityKit
-  BindTarget 

Enumeration

# BindTarget

A reference to a particular scene, entity, or property that animates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum BindTarget
```

## Overview

This structure describes a reference to an animated property. The property may be a transform, collection of joint transforms, an arbitrary named property of an entity, or the property of a nested entity.

For nested entities, the BindTarget.path(_:) case returns a BindPath instance that contains an array of *parts* (BindPath.Part). Each part identifies one or more nested, named entities or scenes, followed by the property to animate.

## Topics

### Choosing a bind target

case `internal`(InternalBindPath)

A bind target that refers to a framework-provided property.

case jointTransforms

An option that specifies that the entity’s joint transforms animate.

case parameter(String)

Provides a property that animates from the given textual name.

case path(BindPath)

Provides a complex bind path capable of animating additional entities other than the current entity.

case transform

A option that specifies that the target entity’s transform animates.

### Comparing bind targets

static func == (BindTarget, BindTarget) -> Bool

Returns a Boolean value that indicates whether two bind targets are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Targeting entities and scenes

static func scene(String) -> BindTarget.ScenePath

Generates a bind path from a particular scene.

struct ScenePath

A bind path for a particular scene.

static func anchorEntity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular anchor entity in the scene.

static func entity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular child entity of the current entity.

struct EntityPath

A bind path context for a particular entity.

### Structures

struct IkSolverPath

struct MaterialPath

Material parameters that an animation can target.

struct TextureCoordinateTransformPath

The texture coordinate parameters for a given texture layer that an animation can target.

### Enumeration Cases

case billboardBlendFactor

case blendShapeWeights

An option the entity’s blend shape weights animate. Requires that the entity has a BlendShapeWeightsComponent.

case blendShapeWeightsAtIndex(Int)

case blendShapeWeightsWithID(BlendShapeWeightsData.ID)

case opacity

An option that specifies that the entity’s opacity to animate. Requires that the entity has an OpacityComponent

case skeletalPose(String)

An option that specifies one of the entity’s skeletal poses to animate.

### Type Methods

static func material(Int) -> BindTarget.MaterialPath

Generates a complex bind path from one of an entity’s materials.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Bindable animation targets

struct BindPath

The components of a target’s path that refer to the animation properties of a nested scene or entity.

struct BindableValue

The value of a bindable target.

struct BindableValuesReference

A reference to a bindable value of an animation.

struct ParameterSet

A reference to general-purpose entity parameters for animations.

struct InternalBindPath

A bind target for framework-provided properties.

