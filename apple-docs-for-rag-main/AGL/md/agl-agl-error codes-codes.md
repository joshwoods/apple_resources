

- AGL
- AGL
-  Error Codes 

API Collection

# Error Codes

Defines the error codes that can be returned by the aglGetError function.

## Overview

Unlike many Carbon APIs, AGL functions don’t return result codes for specific error conditions. Instead, AGL functions that fail either return `GL_FALSE` or `NULL`. You can find out the specific nature of the error by calling the function aglGetError, which returns the appropriate error code.

## Topics

### Constants

var AGL_NO_ERROR: Int32

No error.

var AGL_BAD_ATTRIBUTE: Int32

Invalid pixel format attribute.

var AGL_BAD_PROPERTY: Int32

Invalid renderer property.

var AGL_BAD_PIXELFMT: Int32

Invalid pixel format.

var AGL_BAD_RENDINFO: Int32

Invalid renderer info.

var AGL_BAD_CONTEXT: Int32

Invalid rendering context.

var AGL_BAD_DRAWABLE: Int32

var AGL_BAD_GDEV: Int32

Invalid graphics device.

var AGL_BAD_STATE: Int32

Invalid rendering context state.

var AGL_BAD_VALUE: Int32

Invalid numerical value.

var AGL_BAD_MATCH: Int32

Invalid share rendering context.

var AGL_BAD_ENUM: Int32

Invalid enumerant.

var AGL_BAD_OFFSCREEN: Int32

Invalid offscreen drawable object.

var AGL_BAD_FULLSCREEN: Int32

Invalid full-screen drawable object.

var AGL_BAD_WINDOW: Int32

Invalid window.

var AGL_BAD_POINTER: Int32

Invalid pointer.

var AGL_BAD_MODULE: Int32

Invalid code module.

var AGL_BAD_ALLOC: Int32

Memory allocation failure.

var AGL_BAD_CONNECTION: Int32

Unable to connect to the window server.

var AGL_NO_ERROR: Int32

No error.

var AGL_BAD_ATTRIBUTE: Int32

Invalid pixel format attribute.

var AGL_BAD_PROPERTY: Int32

Invalid renderer property.

var AGL_BAD_PIXELFMT: Int32

Invalid pixel format.

var AGL_BAD_RENDINFO: Int32

Invalid renderer info.

var AGL_BAD_CONTEXT: Int32

Invalid rendering context.

var AGL_BAD_DRAWABLE: Int32

var AGL_BAD_GDEV: Int32

Invalid graphics device.

var AGL_BAD_STATE: Int32

Invalid rendering context state.

var AGL_BAD_VALUE: Int32

Invalid numerical value.

var AGL_BAD_MATCH: Int32

Invalid share rendering context.

var AGL_BAD_ENUM: Int32

Invalid enumerant.

var AGL_BAD_OFFSCREEN: Int32

Invalid offscreen drawable object.

var AGL_BAD_FULLSCREEN: Int32

Invalid full-screen drawable object.

var AGL_BAD_WINDOW: Int32

Invalid window.

var AGL_BAD_POINTER: Int32

Invalid pointer.

var AGL_BAD_MODULE: Int32

Invalid code module.

var AGL_BAD_ALLOC: Int32

Memory allocation failure.

var AGL_BAD_CONNECTION: Int32

Unable to connect to the window server.

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

Globally Configured Options

Specify options that apply globally.

Renderer Attributes

Define options for managing renderers.

Renderer IDs

Define constants that specify hardware and software renderers.

Renderer Properties

Specify constants that you can use to query renderer properties.

