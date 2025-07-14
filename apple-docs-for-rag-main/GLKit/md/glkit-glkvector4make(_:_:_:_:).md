

- GLKit
-  GLKVector4Make(\_:\_:\_:\_:) 

Function

# GLKVector4Make(\_:\_:\_:\_:)

Returns a new four-component vector created from individual component values.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector4Make(
    _ x: Float,
    _ y: Float,
    _ z: Float,
    _ w: Float
) -> GLKVector4
```

## Parameters 

`x`  

The first component.

`y`  

The second component.

`z`  

The third component.

`w`  

The fourth component.

## Return Value

An initialized vector.

## See Also

### Creating Vectors

func GLKVector4MakeWithArray(UnsafeMutablePointer&lt;Float>!) -> GLKVector4

Returns a new four-component vector created from an array of components.

func GLKVector4MakeWithVector3(GLKVector3, Float) -> GLKVector4

Returns a new four-component vector created by combining a three-component vector with a scalar value.

