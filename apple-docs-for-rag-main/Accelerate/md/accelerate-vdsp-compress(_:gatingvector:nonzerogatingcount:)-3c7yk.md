

- Accelerate
- vDSP
-  compress(\_:gatingVector:nonZeroGatingCount:) 

Type Method

# compress(\_:gatingVector:nonZeroGatingCount:)

Returns a compressed copy of the specified single-precision vector using the nonzero values in a gating vector.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func compress(
    _ vector: T,
    gatingVector: U,
    nonZeroGatingCount: Int?
) -> [Float] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Float, U.Element == Float
```

## Parameters 

`vector`  

The source vector that the function compresses.

`gatingVector`  

The gating vector.

`nonZeroGatingCount`  

The number of nonzero elements in `gatingVector`. Set to `nil` to have the operation calculate this value for you.

## Return Value

The result of the compression operation.

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

let destination = vDSP.compress(source,
                                gatingVector: gatingVector,
                                nonZeroGatingCount: nil)

// Prints "[1.0, 3.0, 5.0, 7.0]".
print(destination)
```

## See Also

### Vector compression

static func compress&lt;T, U>(T, gatingVector: U, nonZeroGatingCount: Int?) -> [Double]

Returns a compressed copy of the specified double-precision vector using the nonzero values in a gating vector.

static func compress&lt;T, U, V>(T, gatingVector: U, result: inout V)

Compresses the specified single-precision vector using the nonzero values in a gating vector.

static func compress&lt;T, U, V>(T, gatingVector: U, result: inout V)

Compresses the specified double-precision vector using the nonzero values in a gating vector.

