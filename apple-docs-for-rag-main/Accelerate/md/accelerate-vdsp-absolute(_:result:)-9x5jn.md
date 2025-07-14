

- Accelerate
- vDSP
-  absolute(\_:result:) 

Type Method

# absolute(\_:result:)

Calculates the absolute value of each element in the supplied single-precision complex vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func absolute(
    _ vector: DSPSplitComplex,
    result: inout V
) where V : AccelerateMutableBuffer, V.Element == Float
```

## Parameters 

`vector`  

The source vector.

`result`  

On output, the absolute values of the elements in the source vector.

## Discussion

This function returns the square roots of the sum of the squares of the real and imaginary parts of each complex element.

For example, the following code calculates the absolute values of four complex numbers:

```
    let n = 4

    let reals = UnsafeMutableBufferPointer.allocate(capacity: n)
    _ = reals.initialize(from: [-3, -6, 5, 9])

    let imaginaries = UnsafeMutableBufferPointer.allocate(capacity: n)
    _ = imaginaries.initialize(from: [4, -8, -12, 12])

    let values = DSPSplitComplex(realp: reals.baseAddress!,
                            imagp: imaginaries.baseAddress!)

    let absoluteValues = [Float](unsafeUninitializedCapacity: n) {
        buffer, initializedCount in

        vDSP.absolute(values, result: &buffer)

        initializedCount = n
    }

    // Prints "[5.0, 10.0, 13.0, 15.0]".
    print(absoluteValues)
```

## See Also

### Complex vector absolute functions

static func absolute&lt;V>(DSPDoubleSplitComplex, result: inout V)

Calculates the absolute value of each element in the supplied double-precision complex vector.

