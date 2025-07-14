

- SpriteKit
-  SKShader 

Class

# SKShader

An object that allows you to apply a custom fragment shader.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class SKShader
```

## Mentioned in 

Controlling Shape Drawing with Shaders

Creating a Custom Fragment Shader

Applying Shaders to a Sprite

Creating a New Node By Rendering To a Texture

Getting Started with Particle Shaders

## Overview

An SKShader object holds a custom OpenGL ES fragment shader. Shader objects are used to customize the drawing behavior of many different kinds of nodes in SpriteKit.

To use a custom shader, create an SKShader object and provide the source for the custom fragment shader. If your shader needs to provide uniform data to the shader, create one or more SKUniform objects and associate them with the shader object. If your shader needs to provide per-node data to the shader, create one or more SKAttribute objects and associate them with the relevant nodes. Then, assign the shader object to the shader property of any sprites that need the custom behavior.

Compiling a shader and the uniform data associated with it can be expensive. Because of this, you should:

- Initialize shader objects when your game launches, not while the game is running.

- Avoid changing the shader’s source or changing the list of uniforms or attributes while your game is running. Either of these things recompiles the shader.

- Share shader objects whenever possible. If multiple sprites need the same behavior, create one shader object and associate it with every sprite that needs that behavior. Do not create a separate shader for each sprite.

Important

SKShader does not support OpenGL Extensions. SpriteKit will return an error if you compile a project containing a fragment shader using extensions.

## Topics

### Creating a Shader

Creating a Custom Fragment Shader

Write a fragment shader using the set of SpriteKit-exposed symbols, and supply it with custom data.

convenience init(fileNamed: String)

Creates a new shader object by loading the source for a fragment shader from a file stored in the app’s bundle.

init(source: String, uniforms: [SKUniform])

Initializes a new shader object using the specified source and uniform data.

init(source: String)

Initializes a new shader object using the specified source code.

### Providing Uniform Data to a Shader

func addUniform(SKUniform)

Adds a uniform to the shader.

func removeUniformNamed(String)

Removes a uniform from the shader.

var uniforms: [SKUniform]

The list of uniforms associated with the shader.

func uniformNamed(String) -> SKUniform?

Returns the uniform object corresponding to a particular uniform variable.

### Providing Attribute Data to a Shader

var attributes: [SKAttribute]

The list of attributes associated with the shader.

### Accessing or Setting a Shader’s Source Code

var source: String?

The source code for the shader.

### Executing Shaders in Metal and OpenGL

Executing Shaders in Metal and OpenGL

Toggle between renderers to make sure your shader code compiles in both the Metal and OpenGL environments.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Shaders

class SKAttribute

A specification for dynamic per-node data used with a custom shader.

class SKAttributeValue

A container for dynamic shader data associated with a node.

class SKUniform

A container for uniform shader data.

