

- ARKit
- ARConfiguration
-  ARConfiguration.SceneReconstruction 

Structure

# ARConfiguration.SceneReconstruction

Options that enable ARKit to detect the shape of the physical environment.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
struct SceneReconstruction
```

## Overview

When you set one of the these values onto a world-tracking configuration’s sceneReconstruction property, ARKit provides you with a mesh that models the real-world surrounding the user.

## Topics

### Modeling the Environment

init(rawValue: UInt)

Initializes a scene-reconstruction object.

static var mesh: ARConfiguration.SceneReconstruction

A polygonal mesh approximation of the physical environment.

static var meshWithClassification: ARConfiguration.SceneReconstruction

An approximate shape of the physical environment, including classification of the real-world objects within it.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

