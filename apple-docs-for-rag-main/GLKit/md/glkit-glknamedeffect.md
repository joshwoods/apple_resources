

- GLKit
-  GLKNamedEffect 

Protocol

# GLKNamedEffect

A standard interface for objects that provide shader-based OpenGL rendering effects.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
protocol GLKNamedEffect
```

## Overview

Objects that implement the GLKNamedEffect protocol provide rendering support to shader-based apps. An effect is expected to provide access to one or more shaders. The typical usage pattern for an effect separates initialization tasks from rendering tasks, allowing the effect object to be used efficiently inside an animation loop.

At initialization time, your app first creates a compatible context and makes it current. Then it allocates and initializes a new effect object, configures its properties, and calls its prepareToDraw() method. Preparing an effect causes a shader to be compiled and bound to the current context. When an effect requires vertex data to act as inputs to the shader, your app also creates one or more vertex array objects. For each attribute required by the shader, the vertex array object should enable the attribute and point to data stored in a vertex buffer object.

At runtime, your app calls the effect’s prepareToDraw() method to bind the shader program as the current program. Then, it binds a vertex array object (if necessary) and submits one or more OpenGL drawing commands.

## Topics

### Binding the Shader Program

func prepareToDraw()

Prepares an effect for OpenGL ES rendering.

**Required**

## Relationships

### Conforming Types

- GLKBaseEffect
- GLKReflectionMapEffect
- GLKSkyboxEffect

## See Also

### Shader-Based Rendering Effects

class GLKBaseEffect

A simple lighting and shading system for use in shader-based OpenGL rendering.

Deprecated

class GLKReflectionMapEffect

A lighting and shading system that supports reflection mapping for use in shader-based OpenGL rendering.

Deprecated

class GLKSkyboxEffect

A simple skybox visual effect for use in shader-based OpenGL rendering.

Deprecated

