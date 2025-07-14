

- AppKit
- NSBitmapImageRep
-  colorAt(x:y:) 

Instance Method

# colorAt(x:y:)

Returns the color of the pixel at the specified coordinates.

macOS

``` source
func colorAt(
    x: Int,
    y: Int
) -> NSColor?
```

## Parameters 

`x`  

The x-axis coordinate.

`y`  

The y-axis coordinate.

## Return Value

A color object representing the color at the specified coordinates.

## Discussion

Calling this method creates a new NSColor object. The overhead of object creation means this method is best suited for infrequent color sampling. If you instead need to work with large numbers of pixels, access the bitmap data directly using the bitmapData property or the getPixel(_:atX:y:) method for better performance.

## See Also

### Managing Pixel Values

func setColor(NSColor, atX: Int, y: Int)

Changes the color of the pixel at the specified coordinates.

func setPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Sets the bitmap image representation’s pixel at the specified coordinates to the specified raw pixel values.

func getPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Returns by indirection the pixel data for the specified location in the bitmap image representation.

