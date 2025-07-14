

- Accelerate
- vDSP
-  window(ofType:usingSequence:count:isHalfWindow:) 

Type Method

# window(ofType:usingSequence:count:isHalfWindow:)

Returns an array that contains the specified window.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func window(
    ofType: T.Type,
    usingSequence sequence: vDSP.WindowSequence,
    count: Int,
    isHalfWindow: Bool
) -> [T] where T : vDSP_FloatingPointGeneratable
```

## Parameters 

`ofType`  

The precision of the generated window.

`sequence`  

The window sequence to use for generation.

`count`  

The number of elements to generate.

`isHalfWindow`  

A Boolean value that specifies whether the function generates half of the number of elements.

## Mentioned in 

Reducing spectral leakage with windowing

## Discussion

Use this function to generate and return a vector populated with values of a specified window sequence.

The following code shows how to generate a single-precision Blackman window:

```
let c = vDSP.window(ofType: Float.self,
                    usingSequence: .blackman,
                    count: 1024,
                    isHalfWindow: false)
```

The following figure illustrates the values of the output vector, `c`:

## See Also

### Type Methods

static func absolute&lt;U>(U) -> [Double]

Returns the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U>(U) -> [Float]

Returns the absolute value of each element in the supplied single-precision vector.

static func absolute&lt;V>(DSPSplitComplex, result: inout V)

Calculates the absolute value of each element in the supplied single-precision complex vector.

static func absolute&lt;V>(DSPDoubleSplitComplex, result: inout V)

Calculates the absolute value of each element in the supplied double-precision complex vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied single-precision vector.

static func add&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise sum of two vectors.

static func add&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise sum of two vectors.

static func add&lt;U, V>(Double, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise sum of two vectors.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise sum of two vectors.

static func add(DSPSplitComplex, to: DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the single-precision elementwise sum of the supplied complex vectors.

