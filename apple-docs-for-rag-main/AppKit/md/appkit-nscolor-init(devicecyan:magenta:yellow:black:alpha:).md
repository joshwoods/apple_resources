

- AppKit
- NSColor
-  init(deviceCyan:magenta:yellow:black:alpha:) 

Initializer

# init(deviceCyan:magenta:yellow:black:alpha:)

Creates a color object using the given opacity value and CMYK components.

macOS

``` source
init(
    deviceCyan cyan: CGFloat,
    magenta: CGFloat,
    yellow: CGFloat,
    black: CGFloat,
    alpha: CGFloat
)
```

## Parameters 

`cyan`  

The cyan component of the color object.

`magenta`  

The magenta component of the color object.

`yellow`  

The yellow component of the color object.

`black`  

The black component of the color object.

`alpha`  

The opacity value of the color object.

## Return Value

The color object.

## Discussion

Values below 0.0 are interpreted as 0.0, and values above 1.0 are interpreted as 1.0.

## See Also

### Related Documentation

func getCyan(UnsafeMutablePointer&lt;CGFloat>?, magenta: UnsafeMutablePointer&lt;CGFloat>?, yellow: UnsafeMutablePointer&lt;CGFloat>?, black: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s CMYK and opacity values.

