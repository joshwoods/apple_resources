

- AGL
- AGL
-  Context Options and Parameters 

API Collection

# Context Options and Parameters

Define options and parameters that apply to a specific rendering context.

## Topics

### Constants

var AGL_SWAP_RECT: Int32

var AGL_BUFFER_RECT: Int32

var AGL_SWAP_LIMIT: Int32

Enable or disable the swap asynchronous limit.

var AGL_COLORMAP_TRACKING: Int32

Enable or disable color map tracking.

var AGL_COLORMAP_ENTRY: Int32

The associated value is a color map entry specifies as {`index, r, g, b}`.

var AGL_RASTERIZATION: Int32

Enable or disable all rasterization of 2D and 3D primitives. You can use this option to debug and characterize the performance of an OpenGL driver without actually rendering.

var AGL_SWAP_INTERVAL: Int32

The associated parameter contains one value: the current swap interval setting. A value of `0` specifies not to synchronize to the vertical retrace. All other values indicate to synchronize to the vertical retrace.

var AGL_STATE_VALIDATION: Int32

var AGL_BUFFER_NAME: Int32

The associated value is a buffer name. You can use this option to allow multiple OpenGL contexts to share a buffer.

var AGL_ORDER_CONTEXT_TO_FRONT: Int32

Specifies to order the current rendering context in front of all the other contexts.

var AGL_CONTEXT_SURFACE_ID: Int32

The associated value is the ID of the drawable surface for the rendering context. You can’t set this value because the system sets it. However, you can retrieve the value using the function aglGetInteger.

var AGL_CONTEXT_DISPLAY_ID: Int32

var AGL_SURFACE_ORDER: Int32

The associated value is the position of the OpenGL surface relative to the window. A value of `1` means that the position is above the window; a value of `–1` specifies a position that is below the window.

var AGL_SURFACE_OPACITY: Int32

The associated value specifies the opacity of the OpenGL surface. A value of `1` means the surface is opaque (the default); `0` means completely transparent.

var AGL_CLIP_REGION: Int32

Enables or sets the drawable clipping region. The associated value is a `rgnHandle` data type that defines the clipping region.

var AGL_FS_CAPTURE_SINGLE: Int32

Enables the capture of a single display for full-screen rendering. This option is disabled by default.

var AGL_SURFACE_BACKING_SIZE: Int32

The associated value specifies the width and height of surface backing size.

var AGL_ENABLE_SURFACE_BACKING_SIZE: Int32

Enable or disable the surface backing-size override.

var AGL_SURFACE_VOLATILE: Int32

Flags the surface as a candidate for deletion.

var AGL_SWAP_RECT: Int32

var AGL_BUFFER_RECT: Int32

var AGL_SWAP_LIMIT: Int32

Enable or disable the swap asynchronous limit.

var AGL_COLORMAP_TRACKING: Int32

Enable or disable color map tracking.

var AGL_COLORMAP_ENTRY: Int32

The associated value is a color map entry specifies as {`index, r, g, b}`.

var AGL_RASTERIZATION: Int32

Enable or disable all rasterization of 2D and 3D primitives. You can use this option to debug and characterize the performance of an OpenGL driver without actually rendering.

var AGL_SWAP_INTERVAL: Int32

The associated parameter contains one value: the current swap interval setting. A value of `0` specifies not to synchronize to the vertical retrace. All other values indicate to synchronize to the vertical retrace.

var AGL_STATE_VALIDATION: Int32

var AGL_BUFFER_NAME: Int32

The associated value is a buffer name. You can use this option to allow multiple OpenGL contexts to share a buffer.

var AGL_ORDER_CONTEXT_TO_FRONT: Int32

Specifies to order the current rendering context in front of all the other contexts.

var AGL_CONTEXT_SURFACE_ID: Int32

The associated value is the ID of the drawable surface for the rendering context. You can’t set this value because the system sets it. However, you can retrieve the value using the function aglGetInteger.

var AGL_CONTEXT_DISPLAY_ID: Int32

var AGL_SURFACE_ORDER: Int32

The associated value is the position of the OpenGL surface relative to the window. A value of `1` means that the position is above the window; a value of `–1` specifies a position that is below the window.

var AGL_SURFACE_OPACITY: Int32

The associated value specifies the opacity of the OpenGL surface. A value of `1` means the surface is opaque (the default); `0` means completely transparent.

var AGL_CLIP_REGION: Int32

Enables or sets the drawable clipping region. The associated value is a `rgnHandle` data type that defines the clipping region.

var AGL_FS_CAPTURE_SINGLE: Int32

Enables the capture of a single display for full-screen rendering. This option is disabled by default.

var AGL_SURFACE_BACKING_SIZE: Int32

The associated value specifies the width and height of surface backing size.

var AGL_ENABLE_SURFACE_BACKING_SIZE: Int32

Enable or disable the surface backing-size override.

var AGL_SURFACE_VOLATILE: Int32

Flags the surface as a candidate for deletion.

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

