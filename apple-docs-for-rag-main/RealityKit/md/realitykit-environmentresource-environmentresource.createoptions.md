

- RealityKit
- EnvironmentResource
-  EnvironmentResource.CreateOptions 

Structure

# EnvironmentResource.CreateOptions

A type that controls compression, sampling quality, and cubemap dimensions when creating an environment resource.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct CreateOptions
```

## Overview

The options provide control for balancing memory usage, quality, and processing power when creating an environment’s lighting data.

## Topics

### Creating the options

init(samplingQuality: EnvironmentResource.CreateOptions.SamplingQuality, specularCubeDimension: Int?, compression: EnvironmentResource.Compression)

Creates an environment creation options structure.

### Specifying the quality

enum SamplingQuality

An object for controlling the skybox sampling quality for lighting textures.

### Accessing the option properties

var compression: EnvironmentResource.Compression

The compression to apply to environment textures.

var samplingQuality: EnvironmentResource.CreateOptions.SamplingQuality

The skybox sampling quality for lighting textures.

var specularCubeDimension: Int?

The dimension of the computed specular cubemap for material reflections.

### Comparing the options

static func == (EnvironmentResource.CreateOptions, EnvironmentResource.CreateOptions) -> Bool

Returns a Boolean value indicating whether two values are equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring the resource creation

typealias Compression

The compression to apply when creating an environment resource.

