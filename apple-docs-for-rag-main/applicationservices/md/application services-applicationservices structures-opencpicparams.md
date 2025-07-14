

- Application Services
- ApplicationServices Structures
-  OpenCPicParams 

Structure

# OpenCPicParams

macOS 10.0+

``` source
struct OpenCPicParams
```

## Topics

### Initializers

init()

init(srcRect: Rect, hRes: Fixed, vRes: Fixed, version: Int16, reserved1: Int16, reserved2: Int32)

### Instance Properties

var hRes: Fixed

The best horizontal resolution for the picture. A value of 0x0048000 specifies a horizontal resolution of 72 dpi.

var reserved1: Int16

Reserved; set to 0.

var reserved2: Int32

Reserved; set to 0.

var srcRect: Rect

The optimal bounding rectangle for the resolution indicated by the `hRes` and `vRes` fields. To display a picture at a resolution other than that specified in the `hRes` and `vRes` fields, your application should compute an appropriate destination rectangle by scaling the image’s width and height by the destination resolution divided by the source resolution.

var vRes: Fixed

The best vertical resolution for the picture. A value of 0x0048000 specifies a vertical resolution of 72 dpi.

var version: Int16

Always set this field to -2.

