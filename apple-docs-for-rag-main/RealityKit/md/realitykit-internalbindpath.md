

- RealityKit
-  InternalBindPath 

Structure

# InternalBindPath

A bind target for framework-provided properties.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct InternalBindPath
```

## Overview

This structure defines a bind path for the BindTarget.internal(_:) case. As a reference to framework properties, this bind target hides its path. You can, however, store and assign instances of this structure.

## See Also

### Bindable animation targets

struct BindPath

The components of a target’s path that refer to the animation properties of a nested scene or entity.

enum BindTarget

A reference to a particular scene, entity, or property that animates.

struct BindableValue

The value of a bindable target.

struct BindableValuesReference

A reference to a bindable value of an animation.

struct ParameterSet

A reference to general-purpose entity parameters for animations.

