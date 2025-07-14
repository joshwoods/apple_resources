

- GLKit
-  GLKVector4MakeWithVector3(\_:\_:) 

Function

# GLKVector4MakeWithVector3(\_:\_:)

Returns a new four-component vector created by combining a three-component vector with a scalar value.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector4MakeWithVector3(
    _ vector: GLKVector3,
    _ w: Float
) -> GLKVector4
```

## Parameters 

`vector`  

A vector.

`w`  

The fourth component.

## Return Value

A new vector.

## See Also

### Creating Vectors

func GLKVector4Make(Float, Float, Float, Float) -> GLKVector4

Returns a new four-component vector created from individual component values.

func GLKVector4MakeWithArray(UnsafeMutablePointer&lt;Float>!) -> GLKVector4

Returns a new four-component vector created from an array of components.

