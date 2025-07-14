

- Accelerate
- vDSP
-  compress(\_:gatingVector:result:) 

Type Method

# compress(\_:gatingVector:result:)

Compresses the specified single-precision vector using the nonzero values in a gating vector.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func compress(
    _ vector: T,
    gatingVector: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Float, U.Element == Float, V.Element == Float
```

## Parameters 

`vector`  

The source vector that the function compresses.

`gatingVector`  

The gating vector.

`result`  

The destination vector that receives the result.

## Discussion

The following code shows an example of compressing the values in `source` using the nonzero values in `gatingVector`:

```
let source: [Float] = [1, 2,
                       3, 4,
                       5, 6,
                       7, 8]

let gatingVector: [Float] = [-1, 0,
                             1, 0,
                             0.001, 0,
                             10, 0]

let count = gatingVector.filter {
    !$0.isZero
}.count

let destination = [Float](unsafeUninitializedCapacity: count) {
    buffer, initializedCount in

    vDSP.compress(source,
                  gatingVector: gatingVector,
                  result: &buffer)

    initializedCount = count
}

// Prints "[1.0, 3.0, 5.0, 7.0]".
print(destination)
}
```

## See Also

### Vector compression

static func compress&lt;T, U>(T, gatingVector: U, nonZeroGatingCount: Int?) -> [Float]

Returns a compressed copy of the specified single-precision vector using the nonzero values in a gating vector.

static func compress&lt;T, U>(T, gatingVector: U, nonZeroGatingCount: Int?) -> [Double]

Returns a compressed copy of the specified double-precision vector using the nonzero values in a gating vector.

static func compress&lt;T, U, V>(T, gatingVector: U, result: inout V)

Compresses the specified double-precision vector using the nonzero values in a gating vector.

