

- Virtualization
- VZMacGraphicsDisplayConfiguration
-  init(widthInPixels:heightInPixels:pixelsPerInch:) 

Initializer

# init(widthInPixels:heightInPixels:pixelsPerInch:)

Create a display configuration with the specified pixel dimensions and pixel density.

macOS 12.0+

``` source
init(
    widthInPixels: Int,
    heightInPixels: Int,
    pixelsPerInch: Int
)
```

## Parameters 

`widthInPixels`  

The width of the display, in pixels.

`heightInPixels`  

The height of the display, in pixels.

`pixelsPerInch`  

The pixel density as a number of pixels per inch.

## See Also

### Creating the display configuration

convenience init(for: NSScreen, sizeInPoints: NSSize)

Create a display configuration suitable for showing on the specified screen.

