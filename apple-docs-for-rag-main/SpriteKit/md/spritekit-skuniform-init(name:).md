

- SpriteKit
- SKUniform
-  init(name:) 

Initializer

# init(name:)

Initializes a new uniform object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(name: String)
```

## Parameters 

`name`  

The name used to identify the uniform variable; you use this name inside your shader to read the uniform variable’s value.

## Return Value

An initialized uniform object.

## Discussion

A uniform initialized with this method has no initial type and cannot be used in a shader until it is given an initial value. To set the initial value, use one of the properties defined in SKUniform. After its value is set, its uniformType property is set to match the uniform’s new type. Once set, the type may not be changed.

## See Also

### Creating and Initializing Uniform Objects

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

