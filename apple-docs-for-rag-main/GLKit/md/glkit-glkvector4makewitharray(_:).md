

- GLKit
-  GLKVector4MakeWithArray(\_:) 

Function

# GLKVector4MakeWithArray(\_:)

Returns a new four-component vector created from an array of components.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector4MakeWithArray(_ values: UnsafeMutablePointer!) -> GLKVector4
```

## Parameters 

`values`  

The array containing the component values.

## Return Value

The array

## Discussion

An initialized vector.

## See Also

### Creating Vectors

func GLKVector4Make(Float, Float, Float, Float) -> GLKVector4

Returns a new four-component vector created from individual component values.

func GLKVector4MakeWithVector3(GLKVector3, Float) -> GLKVector4

Returns a new four-component vector created by combining a three-component vector with a scalar value.

