

- Swift
- Float16
-  squareRoot() 

Instance Method

# squareRoot()

Returns the square root of the value, rounded to a representable value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func squareRoot() -> Self
```

## Return Value

The square root of the value.

## Discussion

The following example declares a function that calculates the length of the hypotenuse of a right triangle given its two perpendicular sides.

```
func hypotenuse(_ a: Double, _ b: Double) -> Double {
    return (a * a + b * b).squareRoot()
}

let (dx, dy) = (3.0, 4.0)
let distance = hypotenuse(dx, dy)
// distance == 5.0
```

