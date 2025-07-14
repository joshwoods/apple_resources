

- Accelerate
- vDSP
-  invertedClip(\_:to:result:) 

Type Method

# invertedClip(\_:to:result:)

Calculates a single-precision vector that’s inverted-clipped to the specified range.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func invertedClip(
    _ vector: U,
    to bounds: ClosedRange,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Clipping Operations

static func clip&lt;U>(U, to: ClosedRange&lt;Double>) -> [Double]

Returns the elements of a double-precision vector clipped to the specified range.

static func clip&lt;U>(U, to: ClosedRange&lt;Float>) -> [Float]

Returns the elements of a single-precision vector clipped to the specified range.

static func clip&lt;U, V>(U, to: ClosedRange&lt;Double>, result: inout V)

Calculates the elements of a double-precision vector clipped to the specified range.

static func clip&lt;U, V>(U, to: ClosedRange&lt;Float>, result: inout V)

Calculates the elements of a single-precision vector clipped to the specified range.

static func invertedClip&lt;U>(U, to: ClosedRange&lt;Double>) -> [Double]

Returns a double-precision vector that’s inverted-clipped to the specified range.

static func invertedClip&lt;U>(U, to: ClosedRange&lt;Float>) -> [Float]

Returns a single-precision vector that’s inverted-clipped to the specified range.

static func invertedClip&lt;U, V>(U, to: ClosedRange&lt;Double>, result: inout V)

Calculates a double-precision vector that’s inverted-clipped to the specified range.

