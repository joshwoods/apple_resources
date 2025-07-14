

- AGL
-  AGL_OFFSCREEN 

Global Variable

# AGL_OFFSCREEN

macOS 10.0+

``` source
var AGL_OFFSCREEN: Int32 { get }
```

## Discussion

This constant is a Boolean attribute. If it is present in the attributes array, only renderers that are capable of rendering to an off-screen memory area and have buffer depth exactly equal to the desired buffer depth are considered. Do not supply a value with this constant because its presence in the array implies `true`, and thereby enables the attribute.

If enabled, and if the drawable object currently attached to a rendering context is an offscreen drawable object, the associated values are the width, height, and row bytes of the offscreen memory area. If enabled, and if the drawable object is not an offscreen type, the width, height, and row bytes are each `0`. When the `AGL_OFFSCREEN` attribute is present, the `AGL_CLOSEST_POLICY` attribute is implied.

## See Also

### Constants

var AGL_NONE: Int32

Used to terminate a pixel format attribute list.

var AGL_ALL_RENDERERS: Int32

This constant is a Boolean attribute. If it is present in the attributes array, pixel format selection is open to all available renderers, including debug and special-purpose renderers that are not OpenGL compliant. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_BUFFER_SIZE: Int32

var AGL_LEVEL: Int32

var AGL_RGBA: Int32

var AGL_DOUBLEBUFFER: Int32

This constant is a Boolean attribute. If it is present in the attributes array, only double-buffered pixel formats are considered. Otherwise, only single-buffered pixel formats are considered. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_STEREO: Int32

This constant is a Boolean attribute. If it is present in the attributes array, only stereo pixel formats are considered. Otherwise, only monoscopic pixel formats are considered. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_AUX_BUFFERS: Int32

var AGL_RED_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of red component bits. The value is `0` if the `AGL_RGBA` attribute is `GL_FALSE`. A red buffer that most closely matches the specified size is preferred.

var AGL_GREEN_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of green component bits. The value is `0` if the `AGL_RGBA` attribute is `GL_FALSE`. A green buffer that most closely matches the specified size is preferred.

var AGL_BLUE_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of blue component bits. The value is `0` if the `AGL_RGBA` attribute is `GL_FALSE`. A blue buffer that most closely matches the specified size is preferred.

var AGL_ALPHA_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of alpha component bits. The value is `0` if the `AGL_RGBA` attribute is `GL_FALSE`. An alpha buffer that most closely matches the specified size is preferred.

var AGL_DEPTH_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits in the depth buffer. A depth buffer that most closely matches the specified size is preferred.

var AGL_STENCIL_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits in the stencil buffer. The smallest stencil buffer of at least the specified size is preferred.

var AGL_ACCUM_RED_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits of red stored in the accumulation buffer. A red accumulation buffer that most closely matches the specified size is preferred.

