

- RealityKit
-  BindableValuesReference 

Structure

# BindableValuesReference

A reference to a bindable value of an animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BindableValuesReference
```

## Overview

As the name indicates, this structure doesn’t exhibit copy-on-write behavior because it’s a reference. This is in contrast to the BindableValue structure.

## Topics

### Accessing values

subscript&lt;T>(BindTarget, T.Type) -> BindableValue&lt;T>?

Returns the bindable value at the subscripted index.

## See Also

### Bindable animation targets

struct BindPath

The components of a target’s path that refer to the animation properties of a nested scene or entity.

enum BindTarget

A reference to a particular scene, entity, or property that animates.

struct BindableValue

The value of a bindable target.

struct ParameterSet

A reference to general-purpose entity parameters for animations.

struct InternalBindPath

A bind target for framework-provided properties.

