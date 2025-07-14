

- Swift
- Double
-  isNormal 

Instance Property

# isNormal

A Boolean value indicating whether this instance is normal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isNormal: Bool { get }
```

## Discussion

A *normal* value is a finite number that uses the full precision available to values of a type. Zero is neither a normal nor a subnormal number.

## See Also

### Querying a Double’s State

var isZero: Bool

A Boolean value indicating whether the instance is equal to zero.

var isFinite: Bool

A Boolean value indicating whether this instance is finite.

var isInfinite: Bool

A Boolean value indicating whether the instance is infinite.

var isNaN: Bool

A Boolean value indicating whether the instance is NaN (“not a number”).

var isSignalingNaN: Bool

A Boolean value indicating whether the instance is a signaling NaN.

var isSubnormal: Bool

A Boolean value indicating whether the instance is subnormal.

var isCanonical: Bool

A Boolean value indicating whether the instance’s representation is in its canonical form.

var floatingPointClass: FloatingPointClassification

The classification of this value.

