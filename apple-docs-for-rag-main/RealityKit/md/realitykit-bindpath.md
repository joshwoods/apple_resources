

- RealityKit
-  BindPath 

Structure

# BindPath

The components of a target’s path that refer to the animation properties of a nested scene or entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BindPath
```

## Overview

The following code demonstrates bind target paths with varying numbers of elements. For a multicomponent target, call the BindPath.Part enumeration for each component. The individual elements form the path’s resulting parts array.

```
// Single-component paths:
let target0: BindTarget = .transform
let target1: BindTarget = .jointTransforms
let target2: BindTarget = .parameter("myInt")

// Relative entity path:
let target3: BindTarget = .entity("entityA").entity("entityB").parameter("myInt")

// Root entity path:
let target4: BindTarget = .anchorEntity("entityA").entity("entityB").transform

// Scene path:
let target5: BindTarget = .scene("sceneA").anchorEntity("entityA").entity("entityB").jointTransforms
```

## Topics

### Composing a property identifier

var parts: [BindPath.Part]

An array of the individual components of a complete bind path.

enum Part

An individual piece of a larger path that refers to the target of an animation.

## See Also

### Bindable animation targets

enum BindTarget

A reference to a particular scene, entity, or property that animates.

struct BindableValue

The value of a bindable target.

struct BindableValuesReference

A reference to a bindable value of an animation.

struct ParameterSet

A reference to general-purpose entity parameters for animations.

struct InternalBindPath

A bind target for framework-provided properties.

