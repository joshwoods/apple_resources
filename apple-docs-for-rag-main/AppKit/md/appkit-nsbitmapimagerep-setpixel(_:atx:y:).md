

- AppKit
- NSBitmapImageRep
-  setPixel(\_:atX:y:) 

Instance Method

# setPixel(\_:atX:y:)

Sets the bitmap image representation’s pixel at the specified coordinates to the specified raw pixel values.

macOS

``` source
func setPixel(
    _ p: UnsafeMutablePointer,
    atX x: Int,
    y: Int
)
```

## Parameters 

`p`  

An array of integers representing the raw pixel values. The values must be in an order appropriate to the object’s bitmap format. Small pixel sample values should be passed as an integer value. Floating point values should be cast `int[]`.

`x`  

The x-axis coordinate of the pixel.

`y`  

The y-axis coordinate of the pixel.

## See Also

### Related Documentation

var bitmapFormat: NSBitmapImageRep.Format

The format of the bitmap image representation.

### Managing Pixel Values

func setColor(NSColor, atX: Int, y: Int)

Changes the color of the pixel at the specified coordinates.

func colorAt(x: Int, y: Int) -> NSColor?

Returns the color of the pixel at the specified coordinates.

func getPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Returns by indirection the pixel data for the specified location in the bitmap image representation.

