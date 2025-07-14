

- RealityKit
-  Resource 

Protocol

# Resource

A shared resource you use to configure a component, like a material, mesh, or texture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@preconcurrency
protocol Resource : Sendable
```

## Overview

Resources can be costly to load or create. Share and reuse resources as much as possible.

## Relationships

### Inherits From

- Sendable

### Conforming Types

- AnimationResource
- AudioBufferResource
- AudioFileGroupResource
- AudioFileResource
- AudioResource
- BlendShapeWeightsMapping
- EnvironmentResource
- IKResource
- MeshResource
- PhysicsMaterialResource
- ShapeResource
- TextureResource

## See Also

### Performance improvements

Improving the Performance of a RealityKit App

Measure CPU and GPU utilization to find ways to improve your app’s performance.

Reducing GPU Utilization in Your RealityKit App

Prevent the GPU from limiting your app’s frame rate by reducing the complexity of your render.

Reducing CPU Utilization in Your RealityKit App

Target specific CPU metrics with adjustments to your app and its content.

Construct an immersive environment for visionOS

Build efficient custom worlds for your app.

Passing Metal command objects around your application

Build a system that creates and passes Metal command objects to entities dispatching Metal compute shaders.

