

- RealityKit
- BindTarget
-  BindTarget.EntityPath 

Structure

# BindTarget.EntityPath

A bind path context for a particular entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct EntityPath
```

## Overview

This structure references all the animated properties of an entity.

To access the animated properties of one of the entity’s children, call entity(_:) and pass in the child’s name.

## Topics

### Accessing a bind target

var jointTransforms: BindTarget

A bind target for the entity’s joint transforms.

var transform: BindTarget

A bind target for the entity’s transform.

var `self`: BindTarget

A bind target for the entity.

func parameter(String) -> BindTarget

Provides a bind target for a particular animated property.

### Accessing child-entity paths

func entity(String) -> BindTarget.EntityPath

Provides a child entity’s path.

### Instance Properties

var billboardBlendFactor: BindTarget

var opacity: BindTarget

A bind target for the entity’s opacity.. Requires that the entity has an OpacityComponent

### Instance Methods

func blendShapeWeights() -> BindTarget

A bind target for the entity’s blend shape weights.

func blendShapeWeightsAtIndex(Int) -> BindTarget

func blendShapeWeightsWithID(BlendShapeWeightsData.ID) -> BindTarget

func ikSolver(IKComponent.Solver.ID?) -> BindTarget.IkSolverPath

func material(Int) -> BindTarget.MaterialPath

Provides a specified material’s path.

func skeletalPose(SkeletalPose.ID) -> BindTarget

## See Also

### Targeting entities and scenes

static func scene(String) -> BindTarget.ScenePath

Generates a bind path from a particular scene.

struct ScenePath

A bind path for a particular scene.

static func anchorEntity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular anchor entity in the scene.

static func entity(String) -> BindTarget.EntityPath

Generates a complex bind path from a particular child entity of the current entity.

