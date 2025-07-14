

- Application Services
- ApplicationServices Structures
- PixMap
-  bounds 

Instance Property

# bounds

The boundary rectangle, which links the local coordinate system of a graphics port to QuickDraw's global coordinate system and defines the area of the bit image into which QuickDraw can draw. By default, the boundary rectangle is the entire main screen. Do not use the `value` of this field to determine the size of the screen; instead use the `value` of the `gdRect` field of the GDevice structure for the screen.

macOS 10.0+

``` source
var bounds: Rect
```

