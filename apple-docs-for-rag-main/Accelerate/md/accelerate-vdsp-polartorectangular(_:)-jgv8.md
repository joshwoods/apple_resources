

- Accelerate
- vDSP
-  polarToRectangular(\_:) 

Type Method

# polarToRectangular(\_:)

Returns double-precision rectangular coordinates converted from polar coordinates.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func polarToRectangular(_ polarCoordinates: U) -> [Double] where U : AccelerateBuffer, U.Element == Double
```

## Parameters 

`polarCoordinates`  

The source polar coordinates.

## Discussion

The function calls the underlying vDSP_rectD function to convert the input angle-radius pairs to Cartesian x-y pairs.

The following code shows how to convert an angle-radius pair (with the angle specified in degress) to its rectangular equivalent:

```
    let angle = Measurement(value: 45,
                            unit: UnitAngle.degrees)
        .converted(to: UnitAngle.radians)
        .value

    let radius = sqrt(25.0 + 25.0)

    let polarCoordinates = [radius, angle]

    let rectangularCoordinates = vDSP.polarToRectangular(polarCoordinates)

    // Prints "[5.0, 5.0]".
    print(rectangularCoordinates)
```

## See Also

### Converting polar coordinates to rectangular coordinates

static func polarToRectangular&lt;U>(U) -> [Float]

Returns single-precision rectangular coordinates converted from polar coordinates.

static func convert&lt;U, V>(polarCoordinates: U, toRectangularCoordinates: inout V)

Converts single-precision polar coordinates to rectangular coordinates.

static func convert&lt;U, V>(polarCoordinates: U, toRectangularCoordinates: inout V)

Converts double-precision polar coordinates to rectangular coordinates.

