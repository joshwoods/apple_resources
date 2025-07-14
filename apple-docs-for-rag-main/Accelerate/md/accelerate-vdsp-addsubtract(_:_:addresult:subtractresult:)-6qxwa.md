

- Accelerate
- vDSP
-  addSubtract(\_:\_:addResult:subtractResult:) 

Type Method

# addSubtract(\_:\_:addResult:subtractResult:)

Calculates the single-precision element-wise sum and subtraction of two vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func addSubtract(
    _ vectorA: S,
    _ vectorB: T,
    addResult: inout U,
    subtractResult: inout V
) where S : AccelerateBuffer, T : AccelerateBuffer, U : AccelerateMutableBuffer, V : AccelerateMutableBuffer, S.Element == Float, T.Element == Float, U.Element == Float, V.Element == Float
```

## Parameters 

`vectorA`  

The first input vector, `A`.

`vectorB`  

The second input vector, `B`.

`addResult`  

The addition output vector, `O0`.

`subtractResult`  

The subtraction output vector, `O1`.

## Discussion

This function calculates the addition and subtraction of the first `N` elements of input vectors `A` and `B`, and writes the result to output vector `C`.

```
 for (i = 0; i 

The following code shows an example of using this function:

```
    let count = 5

    let a: [Float] = [10, 20, 30, 40, 50]
    let b: [Float] = [ 1,  2,  3,  4,  5]

    var o0 = [Float](repeating: 0, count: count)
    var o1 = [Float](repeating: 0, count: count)

    vDSP.addSubtract(a, b, addResult: &o0, subtractResult: &o1)

    // Prints the addition result: "[11.0, 22.0, 33.0, 44.0, 55.0]".
    print(o0)

    // Prints the subtraction result: "[9.0, 18.0, 27.0, 36.0, 45.0]".
    print(o1)
```

## See Also

### Addition and Subtraction

static func addSubtract&lt;S, T, U, V>(S, T, addResult: inout U, subtractResult: inout V)

Calculates the double-precision element-wise sum and subtraction of two vectors.

