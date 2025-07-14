

- AppKit
- NSBitmapImageRep
-  setColor(\_:atX:y:) 

Instance Method

# setColor(\_:atX:y:)

Changes the color of the pixel at the specified coordinates.

macOS

``` source
func setColor(
    _ color: NSColor,
    atX x: Int,
    y: Int
)
```

## Parameters 

`color`  

A color object representing the color to be set.

`x`  

The x-axis coordinate of the pixel.

`y`  

The y-axis coordinate of the pixel.

## See Also

### Managing Pixel Values

func colorAt(x: Int, y: Int) -> NSColor?

Returns the color of the pixel at the specified coordinates.

func setPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Sets the bitmap image representation’s pixel at the specified coordinates to the specified raw pixel values.

func getPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Returns by indirection the pixel data for the specified location in the bitmap image representation.

