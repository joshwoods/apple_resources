

- Accelerate
- vImageRGBPrimaries
-  init(red_x:green_x:blue_x:white_x:red_y:green_y:blue_y:white_y:) 

Initializer

# init(red_x:green_x:blue_x:white_x:red_y:green_y:blue_y:white_y:)

Creates a structure that represents the specified chromaticity of primaries defining a color space.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    red_x: Float,
    green_x: Float,
    blue_x: Float,
    white_x: Float,
    red_y: Float,
    green_y: Float,
    blue_y: Float,
    white_y: Float
)
```

## Parameters 

`red_x`  

The red `x` value according to the CIE 1931 color space.

`green_x`  

The green `x` value according to the CIE 1931 color space.

`blue_x`  

The blue `x` value according to the CIE 1931 color space.

`white_x`  

The white point `x` value according to the CIE 1931 color space.

`red_y`  

The red `y` value according to the CIE 1931 color space.

`green_y`  

The green `y` value according to the CIE 1931 color space.

`blue_y`  

The blue `y` value according to the CIE 1931 color space.

`white_y`  

The white point `y` value according to the CIE 1931 color space.

## Return Value

A new RGB primaries structure.

## See Also

### Initializers

init()

Creates an empty RGB primaries structure.

