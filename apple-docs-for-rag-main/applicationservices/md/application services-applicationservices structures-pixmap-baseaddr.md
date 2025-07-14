

- Application Services
- ApplicationServices Structures
- PixMap
-  baseAddr 

Instance Property

# baseAddr

For an onscreen pixel image, a pointer to the first byte of the image. For optimal performance, this should be a multiple of 4. The `baseAddr` field of the `PixMap` record for an offscreen graphics world contains a handle instead of a pointer. Your application should never directly access the `baseAddr` field of the `PixMap` record for an offscreen graphics world.

macOS 10.0+

``` source
var baseAddr: Ptr!
```

