

- Core ML
- MLFeatureValue
-  dictionaryValue 

Instance Property

# dictionaryValue

The underlying dictionary of the feature value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var dictionaryValue: [AnyHashable : NSNumber] { get }
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

var sequenceValue: MLSequence?

The underlying sequence of the feature value.

