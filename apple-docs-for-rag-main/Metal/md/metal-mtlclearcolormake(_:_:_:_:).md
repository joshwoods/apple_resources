

- Metal
-  MTLClearColorMake(\_:\_:\_:\_:) 

Function

# MTLClearColorMake(\_:\_:\_:\_:)

Returns a color value used to clear a color attachment.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func MTLClearColorMake(
    _ red: Double,
    _ green: Double,
    _ blue: Double,
    _ alpha: Double
) -> MTLClearColor
```

## Parameters 

`red`  

The red color channel.

`green`  

The green color channel.

`blue`  

The blue color channel.

`alpha`  

The alpha channel.

## Return Value

A value for clearing a color attachment.

## See Also

### Specifying Clearing Value

var clearColor: MTLClearColor

The color to use when clearing the color attachment.

