

- AppKit
- NSBitmapImageRep
-  bitmapData 

Instance Property

# bitmapData

A pointer to the bitmap data.

macOS

``` source
var bitmapData: UnsafeMutablePointer? { get }
```

## Discussion

For planar data, the value in this property points to the first plane.

## See Also

### Related Documentation

func getPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Returns by indirection the pixel data for the specified location in the bitmap image representation.

### Getting the Bitmap Data

func getBitmapDataPlanes(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>)

Returns by indirection bitmap data of the bitmap image representation separated into planes.

