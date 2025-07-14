

- SpriteKit
- SKUniform
-  init(name:float:) Deprecated

Initializer

# init(name:float:)

Initializes a new uniform object that holds a `3 x 3` matrix of floating-point numbers.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedmacOS 10.8–10.12DeprecatedtvOSDeprecated

``` source
init(
    name: String,
    float value: GLKMatrix3
)
```

## Parameters 

`name`  

The name used to identify the uniform variable; you use this name inside your shader to read the uniform variable’s value.

`value`  

The initial matrix for the uniform variable.

## Return Value

An initialized uniform object whose type is set to SKUniformType.floatMatrix3.

## See Also

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

init(name: String, float: GLKMatrix4)

Initializes a new uniform object that holds a `4 x 4` matrix of floating-point numbers.

Deprecated

init(name: String, texture: SKTexture?)

Initializes a new uniform object that holds a reference to a texture.

