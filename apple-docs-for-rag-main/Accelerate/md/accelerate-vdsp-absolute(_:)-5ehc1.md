

- Accelerate
- vDSP
-  absolute(\_:) 

Type Method

# absolute(\_:)

Returns the absolute value of each element in the supplied single-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func absolute(_ vector: U) -> [Float] where U : AccelerateBuffer, U.Element == Float
```

## Parameters 

`vector`  

The source vector.

## Discussion

For example, the following code calculates the absolute values of the elements of an array:

```
    let values: [Float] = [-1, 2, -3, 4, -5, 6, -7, 8]

    let absoluteValues = vDSP.absolute(values)

    // Prints "[1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0]".
    print(absoluteValues)
```

## See Also

### Vector absolute functions

static func absolute&lt;U>(U) -> [Double]

Returns the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied single-precision vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied double-precision vector.

