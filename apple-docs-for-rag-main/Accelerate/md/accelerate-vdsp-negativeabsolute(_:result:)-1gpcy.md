

- Accelerate
- vDSP
-  negativeAbsolute(\_:result:) 

Type Method

# negativeAbsolute(\_:result:)

Calculates the negative absolute value of each element in the supplied double-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func negativeAbsolute(
    _ vector: U,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Double
```

## Parameters 

`vector`  

The source vector.

`result`  

On output, the negative absolute values of the elements in the source vector.

## Discussion

For example, the following code calculates the negative absolute values of the elements of an array:

```
    let values: [Double] = [-1, 2, -3, 4, -5, 6, -7, 8]

    let negativeAbsoluteValues = [Double](unsafeUninitializedCapacity: values.count) {
        buffer, initializedCount in

        vDSP.negativeAbsolute(values, result: &buffer)

        initializedCount = values.count
    }

    // Prints "[-1.0, -2.0, -3.0, -4.0, -5.0, -6.0, -7.0, -8.0]".
    print(negativeAbsoluteValues)
```

## See Also

### Vector negative absolute functions

static func negativeAbsolute&lt;U>(U) -> [Float]

Returns the negative absolute value of each element in the supplied single-precision vector.

static func negativeAbsolute&lt;U>(U) -> [Double]

Returns the negative absolute value of each element in the supplied double-precision vector.

static func negativeAbsolute&lt;U, V>(U, result: inout V)

Calculates the negative absolute value of each element in the supplied single-precision vector.

