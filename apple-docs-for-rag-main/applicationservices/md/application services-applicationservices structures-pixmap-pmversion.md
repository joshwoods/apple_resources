

- Application Services
- ApplicationServices Structures
- PixMap
-  pmVersion 

Instance Property

# pmVersion

The version number of Color QuickDraw that created this `PixMap` structure. The value of `pmVersion` is normally 0. If `pmVersion` is 4, Color QuickDraw treats the `PixMap` record's `baseAddr` field as 32-bit clean. All other flags are private. Most applications never need to set this field

macOS 10.0+

``` source
var pmVersion: Int16
```

