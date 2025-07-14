

- Application Services
- ApplicationServices Structures
- PixMap
-  pixelType 

Instance Property

# pixelType

The storage format for a pixel image. Indexed pixels are indicated by a value of 0. Direct pixels are specified by a value of `RGBDirect`, or 16. In the `PixMap` record of the GDevice structure for a direct device, this field is set to `RGBDirect` when the screen depth is set.

macOS 10.0+

``` source
var pixelType: Int16
```

