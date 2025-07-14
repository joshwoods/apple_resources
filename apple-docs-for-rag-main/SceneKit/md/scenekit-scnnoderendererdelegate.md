

- SceneKit
-  SCNNodeRendererDelegate 

Protocol

# SCNNodeRendererDelegate

Methods you can implement to use your own custom Metal or OpenGL drawing code to render content for a node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNNodeRendererDelegate : NSObjectProtocol
```

## Overview

Typically, you use a node renderer delegate to perform custom rendering that is anchored at a location in the scene. For example, you can attach a node with a renderer delegate to part of a scene in order to add a special effect rendered using your own Metal or OpenGL drawing code, such as a fluid simulation. To provide a renderer delegate for an SCNNode object, use its rendererDelegate property.

SceneKit performs no rendering of its own for a node with a render delegate, so this protocol is not appropriate for customizing SceneKit’s rendering of geometry and materials. Instead, use methods in the SCNShadable protocol to extend SceneKit’s rendering using shader programs written in the Metal shading language or the OpenGL Shading Language (GLSL).

## Topics

### Customizing the Rendering of a Node

func renderNode(SCNNode, renderer: SCNRenderer, arguments: [String : Any])

Tells the delegate to perform rendering for a node.

## Relationships

### Inherits From

- NSObjectProtocol

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

protocol SCNTechniqueSupport

The common interface for SceneKit objects that support multipass rendering using SCNTechnique objects.

Postprocessing a Scene With Custom Symbols

Create visual effects in a scene by defining a rendering technique with custom symbols.

