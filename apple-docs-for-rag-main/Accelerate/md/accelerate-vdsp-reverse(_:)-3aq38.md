

- Accelerate
- vDSP
-  reverse(\_:) 

Type Method

# reverse(\_:)

Reverses a vector of double-precision values in-place.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func reverse(_ vector: inout V) where V : AccelerateMutableBuffer, V.Element == Double
```

## Parameters 

`vector`  

The vector that the function reverses.

## Discussion

The single- and double-precision reverse(_:) functions reverse the elements of an array.

The following code reverses the elements in the array `values`:

```
var values: [Float] = [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]

vDSP.reverse(&values)

// Prints "[0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0, 8.0, 9.0]".
print(values)
```

## See Also

### Vector reversing functions

static func reverse&lt;V>(inout V)

Reverses a vector of single-precision values in-place.

