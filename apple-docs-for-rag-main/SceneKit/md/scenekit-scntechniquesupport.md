

- SceneKit
-  SCNTechniqueSupport 

Protocol

# SCNTechniqueSupport

The common interface for SceneKit objects that support multipass rendering using SCNTechnique objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNTechniqueSupport : NSObjectProtocol
```

## Overview

Techniques let you specify approaches to rendering a scene that involves multiple drawing passes. For example, you might create a technique that uses a shader program to postprocess a rendered scene on the GPU, creating special effects such as color grading, screen-space ambient occlusion, or motion blur. Different SceneKit objects support techniques in different ways, summarized in Table 1.

| Class | Description |
|----|----|
| SCNView, SCNLayer (macOS), SCNRenderer | Apply effects whenever the scene is rendered. |
| SCNCamera | Apply effects when the camera is the current point of view. |
| SCNLight | Apply effects when the light is enabled. |

## Topics

### Specifying a Technique

var technique: SCNTechnique?

The technique SceneKit uses when rendering the object.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SCNCamera
- SCNLayer
- SCNLight
- SCNRenderer
- SCNView

## See Also

### Renderer Customization

protocol SCNShadable

Methods for customizing SceneKit’s rendering of geometry and materials using Metal or OpenGL shader programs.

class SCNProgram

A complete Metal or OpenGL shader program that replaces SceneKit’s rendering of a geometry or material.

protocol SCNBufferStream

An object that manages a Metal buffer used by a custom shader program.

class SCNTechnique

A specification for augmenting or postprocessing SceneKit’s rendering of a scene using additional drawing passes with custom Metal or OpenGL shaders.

protocol SCNNodeRendererDelegate

Methods you can implement to use your own custom Metal or OpenGL drawing code to render content for a node.

Postprocessing a Scene With Custom Symbols

Create visual effects in a scene by defining a rendering technique with custom symbols.

