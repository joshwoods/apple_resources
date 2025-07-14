

- Core ML
- MLFeatureValue
-  shapedArrayValue(of:) 

Instance Method

# shapedArrayValue(of:)

Returns the underlying shaped array of the feature value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func shapedArrayValue(of type: Scalar.Type) -> MLShapedArray? where Scalar : MLShapedArrayScalar
```

## Parameters 

`type`  

The scalar type of the underlying shaped array.

## See Also

### Accessing the Feature’s Value

var isUndefined: Bool

A Boolean value that indicates whether the feature value is undefined or missing.

var int64Value: Int64

The underlying integer of the feature value.

var doubleValue: Double

The underlying double of the feature value.

var stringValue: String

The underlying string of the feature value.

var imageBufferValue: CVPixelBuffer?

The underlying image of the feature value as a pixel buffer.

var multiArrayValue: MLMultiArray?

The underlying multiarray of the feature value.

var sequenceValue: MLSequence?

The underlying sequence of the feature value.

var dictionaryValue: [AnyHashable : NSNumber]

The underlying dictionary of the feature value.

