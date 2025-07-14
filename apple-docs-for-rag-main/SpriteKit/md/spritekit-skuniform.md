

- SpriteKit
-  SKUniform 

Class

# SKUniform

A container for uniform shader data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class SKUniform
```

## Mentioned in 

Creating a Custom Fragment Shader

## Overview

An SKUniform object is used to hold uniform data for a custom OpenGL or OpenGL ES shader. The uniform data is accessible from all shaders that include the uniform.To use a uniform variable in your shader, create the SKUniform object and set its initial value. Once its value is specified, the uniformType property changes to match the type of the initial value you provided and can never change afterward. To use the uniform object, add it to an SKShader object that needs to access the uniform variable. To update the uniform variable’s value, choose the appropriate property on the uniform object based on the data type it encapsulates.

## Topics

### Creating and Initializing Uniform Objects

init(name: String)

Initializes a new uniform object.

init(name: String, float: Float)

Initializes a new uniform object that holds a floating-point number.

init(name: String, float: GLKVector2)

Initializes a new uniform object that holds a vector of two floating-point numbers.

Deprecated

init(name: String, float: GLKVector3)

Creates and initializes a new uniform object that holds a vector of three floating-point numbers.

Deprecated

init(name: String, float: GLKVector4)

Initializes a new uniform object that holds a vector of four floating-point numbers.

Deprecated

init(name: String, float: GLKMatrix2)

Initializes a new uniform object that holds a `2 x 2` matrix of floating-point numbers.

Deprecated

init(name: String, float: GLKMatrix3)

Initializes a new uniform object that holds a `3 x 3` matrix of floating-point numbers.

Deprecated

init(name: String, float: GLKMatrix4)

Initializes a new uniform object that holds a `4 x 4` matrix of floating-point numbers.

Deprecated

init(name: String, texture: SKTexture?)

Initializes a new uniform object that holds a reference to a texture.

### Reading Information About a Uniform

var name: String

The uniform’s name.

var uniformType: SKUniformType

The uniform object’s data type.

### Reading and Writing an Uniform Object’s Value

You should only read or write the property type that matches the type of the uniform object; it is a programming error to use any of the other properties.

var floatValue: Float

The receiver’s value as a floating-point value.

var floatVector2Value: GLKVector2

The receiver’s value as a vector of two floating-point values.

Deprecated

var floatVector3Value: GLKVector3

The receiver’s value as a vector of three floating-point values.

Deprecated

var floatVector4Value: GLKVector4

The receiver’s value as a vector of four floating-point values.

Deprecated

var floatMatrix2Value: GLKMatrix2

The receiver’s value as a `2 x 2` matrix of floating-point values.

Deprecated

var floatMatrix3Value: GLKMatrix3

The receiver’s value as a `3 x 3` matrix of floating-point values.

Deprecated

var floatMatrix4Value: GLKMatrix4

The receiver’s value as a `4 x 4` matrix of floating-point values.

Deprecated

var textureValue: SKTexture?

The receiver’s value as a SpriteKit texture.

### Constants

enum SKUniformType

An enumerated type to identify the type of a uniform object.

### Initializers

init(name: String, matrixFloat2x2: matrix_float2x2)

init(name: String, matrixFloat3x3: matrix_float3x3)

init(name: String, matrixFloat4x4: matrix_float4x4)

init(name: String, vectorFloat2: vector_float2)

init(name: String, vectorFloat3: vector_float3)

init(name: String, vectorFloat4: vector_float4)

### Instance Properties

var matrixFloat2x2Value: matrix_float2x2

var matrixFloat3x3Value: matrix_float3x3

var matrixFloat4x4Value: matrix_float4x4

var vectorFloat2Value: vector_float2

var vectorFloat3Value: vector_float3

var vectorFloat4Value: vector_float4

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

class SKShader

An object that allows you to apply a custom fragment shader.

class SKAttribute

A specification for dynamic per-node data used with a custom shader.

class SKAttributeValue

A container for dynamic shader data associated with a node.

