

- SceneKit
-  SCNBufferStream 

Protocol

# SCNBufferStream

An object that manages a Metal buffer used by a custom shader program.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNBufferStream : NSObjectProtocol
```

## Overview

Your app does not define classes that implement this protocol. Instead, you use the SCNProgram method handleBinding(ofBufferNamed:frequency:handler:) to register a block to be called by SceneKit. In that block, SceneKit provides a buffer stream object that you can use to write data to the buffer.

## Topics

### Writing Data to a Buffer

func writeBytes(UnsafeRawPointer, count: Int)

Copies the specified data bytes into the underlying Metal buffer for use by a shader.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Renderer Customization

protocol SCNShadable

Methods for customizing SceneKit’s rendering of geometry and materials using Metal or OpenGL shader programs.

class SCNProgram

A complete Metal or OpenGL shader program that replaces SceneKit’s rendering of a geometry or material.

class SCNTechnique

A specification for augmenting or postprocessing SceneKit’s rendering of a scene using additional drawing passes with custom Metal or OpenGL shaders.

protocol SCNTechniqueSupport

The common interface for SceneKit objects that support multipass rendering using SCNTechnique objects.

protocol SCNNodeRendererDelegate

Methods you can implement to use your own custom Metal or OpenGL drawing code to render content for a node.

Postprocessing a Scene With Custom Symbols

Create visual effects in a scene by defining a rendering technique with custom symbols.

