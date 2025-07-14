

- Accelerate
- vDSP
-  rectangularToPolar(\_:) 

Type Method

# rectangularToPolar(\_:)

Returns single-precision polar coordinates converted from rectangular coordinates.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func rectangularToPolar(_ rectangularCoordinates: U) -> [Float] where U : AccelerateBuffer, U.Element == Float
```

## Parameters 

`rectangularCoordinates`  

The source rectangular coordinates.

## Discussion

The function calls the underlying vDSP_polarD function to convert the input angle-radius pairs to Cartesian x-y pairs.

The following code shows how to convert a set of Cartesian coordinates to its angle-radius pair (with the angle specified in degress) equivalent:

```
   let rectangularCoordinates: [Float] = [ 5.0, 5.0 ]

    let polarCoordinates = vDSP.rectangularToPolar(rectangularCoordinates)

    let radius = polarCoordinates[0]
    let angle = Measurement(value: Double(polarCoordinates[1]),
                            unit: UnitAngle.radians)
        .converted(to: UnitAngle.degrees)
        .value

    // Prints "7.07 45.0".
    print(radius, angle)

```

## See Also

### Converting rectangular coordinates to polar coordinates

static func rectangularToPolar&lt;U>(U) -> [Double]

Returns double-precision polar coordinates converted from rectangular coordinates.

static func convert&lt;U, V>(rectangularCoordinates: U, toPolarCoordinates: inout V)

Converts single-precision rectangular coordinates to polar coordinates.

static func convert&lt;U, V>(rectangularCoordinates: U, toPolarCoordinates: inout V)

Converts double-precision rectangular coordinates to polar coordinates.

