

- RealityKit
-  BindableValue 

Structure

# BindableValue

The value of a bindable target.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BindableValue where T : BindableData
```

## Overview

This structure holds the value of an animatable property (animatedValue), that is, the target property that animates. In addition, the structure stores the property’s original value (baseValue), which represents the property’s value before a running animation starts. The value property returns the animated value when an animation runs; when the animation isn’t running, it returns the base value.

## Topics

### Creating a value

init(T, animatedValue: T?)

Creates a bindable value.

### Accessing the value

var value: T

The main accessor for the bind value.

var baseValue: T

A value that reflects the state of the animated property before or after an animation.

var animatedValue: T?

A value that represents the state of the animated property as an animation progresses.

## See Also

### Bindable animation targets

struct BindPath

The components of a target’s path that refer to the animation properties of a nested scene or entity.

enum BindTarget

A reference to a particular scene, entity, or property that animates.

struct BindableValuesReference

A reference to a bindable value of an animation.

struct ParameterSet

A reference to general-purpose entity parameters for animations.

struct InternalBindPath

A bind target for framework-provided properties.

