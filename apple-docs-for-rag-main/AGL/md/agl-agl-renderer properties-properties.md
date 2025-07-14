

- AGL
- AGL
-  Renderer Properties 

API Collection

# Renderer Properties

Specify constants that you can use to query renderer properties.

## Overview

You can pass these constants to the function AGL to find out the property value for a specific renderer.

## Topics

### Constants

var AGL_BUFFER_MODES: Int32

The associated value can be a bitwise `OR` of the any of the constants specified in Buffer Mode Flags.

var AGL_MIN_LEVEL: Int32

The associated value specifies the minimum overlay buffer level. Negative values indicate an underlay buffer.

var AGL_MAX_LEVEL: Int32

The associated value specifies the maximum overlay buffer level.

var AGL_COLOR_MODES: Int32

The associated value can be a bitwise `OR` of any of the constants specified in Color Modes.

var AGL_ACCUM_MODES: Int32

The associated value can be a bitwise `OR` of any of the constants specified in Color Modes.

var AGL_DEPTH_MODES: Int32

The associated value can be the bitwise `OR` of any of the constants specified in Bit Depths.

var AGL_STENCIL_MODES: Int32

The associated value can be the bitwise `OR` of any of the constants specified in Bit Depths.

var AGL_MAX_AUX_BUFFERS: Int32

The associated value is the maximum number of auxiliary buffers that can be supported by the renderer.

var AGL_VIDEO_MEMORY: Int32

The associated value is the amount of video memory.

var AGL_TEXTURE_MEMORY: Int32

The associated value is the amount of texture memory.

var AGL_RENDERER_COUNT: Int32

The associated value is the number of renderers.

var AGL_BUFFER_MODES: Int32

The associated value can be a bitwise `OR` of the any of the constants specified in Buffer Mode Flags.

var AGL_MIN_LEVEL: Int32

The associated value specifies the minimum overlay buffer level. Negative values indicate an underlay buffer.

var AGL_MAX_LEVEL: Int32

The associated value specifies the maximum overlay buffer level.

var AGL_COLOR_MODES: Int32

The associated value can be a bitwise `OR` of any of the constants specified in Color Modes.

var AGL_ACCUM_MODES: Int32

The associated value can be a bitwise `OR` of any of the constants specified in Color Modes.

var AGL_DEPTH_MODES: Int32

The associated value can be the bitwise `OR` of any of the constants specified in Bit Depths.

var AGL_STENCIL_MODES: Int32

The associated value can be the bitwise `OR` of any of the constants specified in Bit Depths.

var AGL_MAX_AUX_BUFFERS: Int32

The associated value is the maximum number of auxiliary buffers that can be supported by the renderer.

var AGL_VIDEO_MEMORY: Int32

The associated value is the amount of video memory.

var AGL_TEXTURE_MEMORY: Int32

The associated value is the amount of texture memory.

var AGL_RENDERER_COUNT: Int32

The associated value is the number of renderers.

## See Also

### Constants

Bit Depths

Define resolutions for the depth and stencil buffers.

Buffer and Renderer Attributes

Specify attributes used to create a pixel format object.

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

