

- Accelerate
- vForce
-  pow(bases:exponents:result:) 

Type Method

# pow(bases:exponents:result:)

Calculates each double-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func pow(
    bases: T,
    exponents: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Double, U.Element == Double, V.Element == Double
```

## See Also

### Array-Oriented Power Functions

static func pow&lt;U, V>(bases: U, exponents: V) -> [Double]

Returns each double-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;U, V>(bases: U, exponents: V) -> [Float]

Returns each single-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;T, U, V>(bases: T, exponents: U, result: inout V)

Calculates each single-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

func vvpow(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Raises each element in an array to the power of the corresponding element in a second array of double-precision values.

func vvpowf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Raises each element in an array to the power of the corresponding element in a second array of single-precision values.

