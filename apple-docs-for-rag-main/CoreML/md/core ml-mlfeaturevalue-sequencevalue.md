

- Core ML
- MLFeatureValue
-  sequenceValue 

Instance Property

# sequenceValue

The underlying sequence of the feature value.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var sequenceValue: MLSequence? { get }
```

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

func shapedArrayValue&lt;Scalar>(of: Scalar.Type) -> MLShapedArray&lt;Scalar>?

Returns the underlying shaped array of the feature value.

var multiArrayValue: MLMultiArray?

The underlying multiarray of the feature value.

var dictionaryValue: [AnyHashable : NSNumber]

The underlying dictionary of the feature value.

