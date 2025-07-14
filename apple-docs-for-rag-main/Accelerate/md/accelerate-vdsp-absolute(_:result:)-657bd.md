

- Accelerate
- vDSP
-  absolute(\_:result:) 

Type Method

# absolute(\_:result:)

Calculates the absolute value of each element in the supplied double-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func absolute(
    _ vector: U,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Double
```

## Parameters 

`vector`  

The source vector.

`result`  

On output, the absolute values of the elements in the source vector.

## Discussion

For example, the following code calculates the absolute values of the elements of an array:

```
    let values: [Double] = [-1, 2, -3, 4, -5, 6, -7, 8]

    let absoluteValues = [Double](unsafeUninitializedCapacity: values.count) {
        buffer, initializedCount in

        vDSP.absolute(values, result: &buffer)

        initializedCount = values.count
    }

    // Prints "[1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0]".
    print(absoluteValues)
```

## See Also

### Vector absolute functions

static func absolute&lt;U>(U) -> [Float]

Returns the absolute value of each element in the supplied single-precision vector.

static func absolute&lt;U>(U) -> [Double]

Returns the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied single-precision vector.

