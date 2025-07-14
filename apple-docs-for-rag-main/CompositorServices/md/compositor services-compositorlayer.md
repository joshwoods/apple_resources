

- Compositor Services
-  CompositorLayer 

Structure

# CompositorLayer

A type that you use with an immersive space to display fully immersive content using Metal.

CompositorServicesSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
struct CompositorLayer
```

## Mentioned in 

Drawing fully immersive content using Metal

## Overview

Use a CompositorLayer to specify the content of an ImmersiveSpace when you want to render that content yourself using Metal. When you present a space with this content, Compositor Services creates a LayerRenderer type for you to use with your rendering code. The layer renderer provides configuration details, timing information, and the Metal types and information you need to configure your rendering loop and manage the rendering process.

The following example shows a ImmersiveSpace that uses a CompositorLayer to specify its content. Use the closure for the CompositorLayer to set up and start your Metal rendering code. In this example, Compositor Services creates the layer using a default set of Metal configuration options. To customize the configuration of your Metal rendering environment, pass a custom CompositorLayerConfiguration type to your CompositorLayer at initialization time.

```
```

For more information about how to set up and start your Metal rendering engine, see Drawing fully immersive content using Metal.

## Topics

### Initializers

init(configuration: any CompositorLayerConfiguration, renderer: (LayerRenderer) -> Void)

init(configuration: any CompositorLayerConfiguration, renderer: (LayerRenderer) -> Void, Void)Deprecated

## Relationships

### Conforms To

- ImmersiveSpaceContent
- Sendable

## See Also

### App integration

Drawing fully immersive content using Metal

Create a fully immersive experience in visionOS using a custom Metal-based rendering engine.

Interacting with virtual content blended with passthrough

Present a mixed immersion style space to draw content in a person’s surroundings, and choose how upper limbs appear with respect to rendered content.

protocol CompositorLayerConfiguration

An interface for specifying the texture configurations and rendering behaviors to use with your Metal rendering engine.

struct DefaultCompositorLayerConfiguration

A type that configures the layer with the default texture configurations and rendering behaviors for the current device.

