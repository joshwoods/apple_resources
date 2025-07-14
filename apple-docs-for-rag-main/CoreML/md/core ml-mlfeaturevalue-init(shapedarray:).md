

- Core ML
- MLFeatureValue
-  init(shapedArray:) 

Initializer

# init(shapedArray:)

Creates a feature value that contains a shaped array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(shapedArray: MLShapedArray) where Scalar : MLShapedArrayScalar
```

## Parameters 

`shapedArray`  

An MLShapedArray instance.

## See Also

### Creating Multidimensional Feature Values

convenience init(multiArray: MLMultiArray)

Creates a feature value that contains a multidimensional array.

