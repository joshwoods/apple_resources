

- Accelerate
- vDSP
-  gather(\_:indices:result:) 

Type Method

# gather(\_:indices:result:)

Gathers the specified double-precision vector using a vector that defines the indices to keep.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func gather(
    _ vector: T,
    indices: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Double, U.Element == UInt, V.Element == Double
```

## Parameters 

`vector`  

The source vector that the function gathers.

`indices`  

The vector that contains the one-based indices.

`result`  

The destination vector that receives the result.

## Discussion

The following code shows an example of gathering the values in `source` using the values in `indices`:

```
let source: [Double] = [10, 20,
                        30, 40,
                        50, 60,
                        70, 80]

let indices: [UInt] = [1, 3, 5, 7]

let count = indices.count

let destination = [Double](unsafeUninitializedCapacity: count) {
    buffer, initializedCount in

    vDSP.gather(source,
                indices: indices,
                result: &buffer)

    initializedCount = count
}

// Prints "[10.0, 30.0, 50.0, 70.0]".
print(destination)
```

## See Also

### Vector gathering functions

static func gather&lt;T, U>(T, indices: U) -> [Float]

Returns a gathered copy of the specified single-precision vector using a vector that defines the indices to keep.

static func gather&lt;T, U>(T, indices: U) -> [Double]

Returns a gathered copy of the specified double-precision vector using a vector that defines the indices to keep.

static func gather&lt;T, U, V>(T, indices: U, result: inout V)

Gathers the specified single-precision vector using a vector that defines the indices to keep.

