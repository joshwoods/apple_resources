

- SpriteKit
- SKAttributeValue
-  vectorFloat3Value 

Instance Property

# vectorFloat3Value

The receiver’s value as a vector of three floating point numbers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var vectorFloat3Value: vector_float3 { get set }
```

## Discussion

If the receiver’s original value is a floating-point number or a vector_float2, the empty items in the vector are set to 0. If the receiver’s original value is a vector_float4, the last item is truncated.

## See Also

### Instance Properties

var floatValue: Float

The receiver’s floating point value.

var vectorFloat2Value: vector_float2

The receiver’s value as a vector of two floating-point numbers.

var vectorFloat4Value: vector_float4

The receiver’s value as a vector of four floating point numbers.

