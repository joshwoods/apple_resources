

- Core ML
- MLSendableFeatureValue
-  shapedArrayValue(of:) 

Instance Method

# shapedArrayValue(of:)

Returns the shaped array value, if the contained value is a shaped array of the specified type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func shapedArrayValue(of type: Scalar.Type) -> MLShapedArray? where Scalar : MLShapedArrayScalar
```

