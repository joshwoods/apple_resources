

- AppKit
- NSBitmapImageRep
-  getPixel(\_:atX:y:) 

Instance Method

# getPixel(\_:atX:y:)

Returns by indirection the pixel data for the specified location in the bitmap image representation.

macOS

``` source
func getPixel(
    _ p: UnsafeMutablePointer,
    atX x: Int,
    y: Int
)
```

## Parameters 

`p`  

On return, an array of integers containing raw pixel data in the appropriate order according to the object’s bitmap format. Smaller integer samples, such as 4-bit, are returned as an integer. Floating point values are cast to integer values and returned.

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

func setPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Sets the bitmap image representation’s pixel at the specified coordinates to the specified raw pixel values.

