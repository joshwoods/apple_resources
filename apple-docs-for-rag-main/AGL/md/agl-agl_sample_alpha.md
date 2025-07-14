

- AGL
-  AGL_SAMPLE_ALPHA 

Global Variable

# AGL_SAMPLE_ALPHA

This constant is a Boolean attribute. If it is present in the attributes array, request alpha filtering when multisampling. Do not supply a value with this constant because its presence in the array implies `true`.

macOS 10.0+

``` source
var AGL_SAMPLE_ALPHA: Int32 { get }
```

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

