

- AppKit
- NSBitmapImageRep
-  cgImage 

Instance Property

# cgImage

A Core Graphics image object based on the bitmap image representation’s data.

macOS 10.5+

``` source
var cgImage: CGImage? { get }
```

## Discussion

The autoreleased CGImage opaque type in this property has pixel dimensions that are identical to those of the bitmap image rep object. If an existing CGImage opaque type is not available, accessing this property creates a new one. If you change the bitmap image rep’s contents later, accessing this property again might return a different CGImage opaque type.

## See Also

### Related Documentation

init(cgImage: CGImage)

Returns a bitmap image representation from a Core Graphics image object.

