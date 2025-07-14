

- RealityKit
- MaterialParameterTypes
-  MaterialParameterTypes.TextureCoordinateTransform 

Structure

# MaterialParameterTypes.TextureCoordinateTransform

An object that defines a transformation the framework applies to a material’s UV-mapped textures.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct TextureCoordinateTransform
```

## Overview

An entity’s UV texture coordinates define how RealityKit maps image textures onto an entity. This object defines a transformation to texture coordinates that changes the way this material maps textures onto an entity. You might, for example, continuously rotate, translate, or scale the texture coordinates and animate materials to create special effects, such as fire or flowing liquids.

## Topics

### Creating a texture coordinate transform

init(offset: SIMD2&lt;Float>, scale: SIMD2&lt;Float>, rotation: Float)

Creates a texture coordinate transform object.

### Accessing the transform values

var offset: SIMD2&lt;Float>

The amount by which the framework offsets the entity’s UV texture coordinates.

var scale: SIMD2&lt;Float>

The amount by which the framework scale the UV texture coordinates.

var rotation: Float

The amount by which the framework rotates the UV texture coordinates you specify in radians.

