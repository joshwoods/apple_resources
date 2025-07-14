

- AGL
- AGL
-  Buffer and Renderer Attributes 

API Collection

# Buffer and Renderer Attributes

Specify attributes used to create a pixel format object.

## Overview

Each of these constants can be assigned to the the attribute array passed to the function AGL. They can also be passed to the function AGL.

## Topics

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

var AGL_ACCUM_GREEN_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits of green stored in the accumulation buffer. A green accumulation buffer that most closely matches the specified size is preferred.

var AGL_ACCUM_BLUE_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits of blue stored in the accumulation buffer. A blue accumulation buffer that most closely matches the specified size is preferred.

var AGL_ACCUM_ALPHA_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits of alpha stored in the accumulation buffer. An alpha accumulation buffer that most closely matches the specified size is preferred.

var AGL_PIXEL_SIZE: Int32

var AGL_MINIMUM_POLICY: Int32

This constant is a Boolean attribute. If it is present in the attributes array, the pixel format choosing policy is altered for the color, depth, and accumulation buffers such that only buffers of size greater than or equal to the desired size are considered. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_MAXIMUM_POLICY: Int32

var AGL_OFFSCREEN: Int32

var AGL_FULLSCREEN: Int32

var AGL_SAMPLE_BUFFERS_ARB: Int32

The associated value is the number of multisample buffers.

var AGL_SAMPLES_ARB: Int32

The associated value is the number of samples per multisample buffer.

var AGL_AUX_DEPTH_STENCIL: Int32

The associated value is the independent depth and/or the stencil buffers for the auxiliary buffer.

var AGL_COLOR_FLOAT: Int32

This constant is a Boolean attribute. If it is present in the attributes array, color buffers store floating-point pixels. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_MULTISAMPLE: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies a hint to the driver to prefer multisampling. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_SUPERSAMPLE: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies a hint to the driver to prefer supersampling. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_SAMPLE_ALPHA: Int32

This constant is a Boolean attribute. If it is present in the attributes array, request alpha filtering when multisampling. Do not supply a value with this constant because its presence in the array implies `true`.

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

var AGL_ACCUM_GREEN_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits of green stored in the accumulation buffer. A green accumulation buffer that most closely matches the specified size is preferred.

var AGL_ACCUM_BLUE_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits of blue stored in the accumulation buffer. A blue accumulation buffer that most closely matches the specified size is preferred.

var AGL_ACCUM_ALPHA_SIZE: Int32

The associated value is a nonnegative integer that specifies the number of bits of alpha stored in the accumulation buffer. An alpha accumulation buffer that most closely matches the specified size is preferred.

var AGL_PIXEL_SIZE: Int32

var AGL_MINIMUM_POLICY: Int32

This constant is a Boolean attribute. If it is present in the attributes array, the pixel format choosing policy is altered for the color, depth, and accumulation buffers such that only buffers of size greater than or equal to the desired size are considered. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_MAXIMUM_POLICY: Int32

var AGL_OFFSCREEN: Int32

var AGL_FULLSCREEN: Int32

var AGL_SAMPLE_BUFFERS_ARB: Int32

The associated value is the number of multisample buffers.

var AGL_SAMPLES_ARB: Int32

The associated value is the number of samples per multisample buffer.

var AGL_AUX_DEPTH_STENCIL: Int32

The associated value is the independent depth and/or the stencil buffers for the auxiliary buffer.

var AGL_COLOR_FLOAT: Int32

This constant is a Boolean attribute. If it is present in the attributes array, color buffers store floating-point pixels. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_MULTISAMPLE: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies a hint to the driver to prefer multisampling. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_SUPERSAMPLE: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies a hint to the driver to prefer supersampling. Do not supply a value with this constant because its presence in the array implies `true`.

var AGL_SAMPLE_ALPHA: Int32

This constant is a Boolean attribute. If it is present in the attributes array, request alpha filtering when multisampling. Do not supply a value with this constant because its presence in the array implies `true`.

## See Also

### Constants

Bit Depths

Define resolutions for the depth and stencil buffers.

Buffer Mode Flags

Define constants used to set buffer modes.

Color Modes

Specify formats and color channel layout information for the color buffer.

Context Options and Parameters

Define options and parameters that apply to a specific rendering context.

Error Codes

Defines the error codes that can be returned by the aglGetError function.

Globally Configured Options

Specify options that apply globally.

Renderer Attributes

Define options for managing renderers.

Renderer IDs

Define constants that specify hardware and software renderers.

Renderer Properties

Specify constants that you can use to query renderer properties.

