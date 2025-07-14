

- Compositor Services
-  CompositorLayerConfiguration 

Protocol

# CompositorLayerConfiguration

An interface for specifying the texture configurations and rendering behaviors to use with your Metal rendering engine.

CompositorServicesSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
protocol CompositorLayerConfiguration
```

## Mentioned in 

Drawing fully immersive content using Metal

## Overview

If you use a custom configuration for your Metal rendering engine, adopt this protocol in a custom type and use it to specify the configuration options you need. In your custom type, implement the makeConfiguration(capabilities:configuration:) method and use it to modify the default set of rendering options. When specifying your configuration, validate choices against the actual capabilities of the current device.

For information on how to specify custom configuration options for your rendering engine, see Drawing fully immersive content using Metal.

## Topics

### Specifying the custom options

func makeConfiguration(capabilities: LayerRenderer.Capabilities, configuration: inout LayerRenderer.Configuration)

Creates and returns a type that contains the rendering options for Compositor Services to use when configuring a layer.

**Required**

### Getting the default options

static var `default`: DefaultCompositorLayerConfiguration

The default configuration options that Compositor Services uses to configure the layer.

## Relationships

### Conforming Types

- DefaultCompositorLayerConfiguration

## See Also

### App integration

Drawing fully immersive content using Metal

Create a fully immersive experience in visionOS using a custom Metal-based rendering engine.

Interacting with virtual content blended with passthrough

Present a mixed immersion style space to draw content in a person’s surroundings, and choose how upper limbs appear with respect to rendered content.

struct CompositorLayer

A type that you use with an immersive space to display fully immersive content using Metal.

struct DefaultCompositorLayerConfiguration

A type that configures the layer with the default texture configurations and rendering behaviors for the current device.

