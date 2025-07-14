

- Accelerate
- vDSP
-  convert(polarCoordinates:toRectangularCoordinates:) 

Type Method

# convert(polarCoordinates:toRectangularCoordinates:)

Converts single-precision polar coordinates to rectangular coordinates.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convert(
    polarCoordinates: U,
    toRectangularCoordinates rectangularCoordinates: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## Parameters 

`polarCoordinates`  

The source polar coordinates.

`rectangularCoordinates`  

On output, the rectangular coordinates.

## Discussion

The function calls the underlying vDSP_rect function to convert the input angle-radius pairs to Cartesian x-y pairs.

The following code shows how to convert an angle-radius pair (with the angle specified in degress) to its rectangular equivalent:

```
    let angle = Measurement(value: 45,
                            unit: UnitAngle.degrees)
        .converted(to: UnitAngle.radians)
        .value

    let radius = sqrt(25.0 + 25.0)

    let polarCoordinates = [radius, angle].map { Float($0) }

    let rectangularCoordinates = [Float](unsafeUninitializedCapacity: 2) {
        buffer,initializedCount in

        vDSP.convert(
            polarCoordinates: polarCoordinates,
            toRectangularCoordinates: &buffer
        )

        initializedCount = 2
    }

    // Prints "[5.0, 5.0]".
    print(rectangularCoordinates)
```

## See Also

### Converting polar coordinates to rectangular coordinates

static func polarToRectangular&lt;U>(U) -> [Float]

Returns single-precision rectangular coordinates converted from polar coordinates.

static func polarToRectangular&lt;U>(U) -> [Double]

Returns double-precision rectangular coordinates converted from polar coordinates.

static func convert&lt;U, V>(polarCoordinates: U, toRectangularCoordinates: inout V)

Converts double-precision polar coordinates to rectangular coordinates.

