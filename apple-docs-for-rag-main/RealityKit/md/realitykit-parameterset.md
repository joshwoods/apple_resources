

- RealityKit
-  ParameterSet 

Structure

# ParameterSet

A reference to general-purpose entity parameters for animations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct ParameterSet
```

## Overview

Subscript this structure to access a particular property by name. The return value is BindableValue ``, where `T` is one of the adopting BindableData types.

As a reference, this structure doesn’t exhibit copy-on-write behavior.

## Topics

### Accessing a parameter by name

subscript&lt;T>(String, T.Type) -> BindableValue&lt;T>?

Provides a bindable value for the given name.

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

struct InternalBindPath

A bind target for framework-provided properties.

