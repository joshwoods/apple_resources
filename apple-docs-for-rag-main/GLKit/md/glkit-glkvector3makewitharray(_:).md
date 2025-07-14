

- GLKit
-  GLKVector3MakeWithArray(\_:) 

Function

# GLKVector3MakeWithArray(\_:)

Returns a new three-component vector created from an array of components.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKVector3MakeWithArray(_ values: UnsafeMutablePointer!) -> GLKVector3
```

## Parameters 

`values`  

The array containing the component values.

## Return Value

The array.

## Discussion

An initialized vector.

## See Also

### Creating Vectors

func GLKVector3Make(Float, Float, Float) -> GLKVector3

Returns a new three-component vector created from individual component values.

