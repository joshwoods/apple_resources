

- Compositor Services
-  DefaultCompositorLayerConfiguration 

Structure

# DefaultCompositorLayerConfiguration

A type that configures the layer with the default texture configurations and rendering behaviors for the current device.

CompositorServicesSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
struct DefaultCompositorLayerConfiguration
```

## Overview

Use this type when your Metal rendering engine uses the default rendering options.

## Relationships

### Conforms To

- CompositorLayerConfiguration
- Sendable

## See Also

### App integration

Drawing fully immersive content using Metal

Create a fully immersive experience in visionOS using a custom Metal-based rendering engine.

Interacting with virtual content blended with passthrough

Present a mixed immersion style space to draw content in a person’s surroundings, and choose how upper limbs appear with respect to rendered content.

struct CompositorLayer

A type that you use with an immersive space to display fully immersive content using Metal.

protocol CompositorLayerConfiguration

An interface for specifying the texture configurations and rendering behaviors to use with your Metal rendering engine.

