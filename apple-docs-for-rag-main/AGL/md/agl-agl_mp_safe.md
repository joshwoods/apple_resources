

- AGL
-  AGL_MP_SAFE 

Global Variable

# AGL_MP_SAFE

macOS 10.0+

``` source
var AGL_MP_SAFE: Int32 { get }
```

## Discussion

This constant is a Boolean attribute. If it is present in the attributes array, specifies a renderer that is multiprocessor safe. This attribute is deprecated in macOS because all renderers can accept commands for threads running on a second processor. However, this does not mean that all renderers are thread-safe or reentrant.

## See Also

### Constants

var AGL_RENDERER_ID: Int32

The associated value is a nonnegative integer that specifies a renderer. If present, OpenGL renderers that match the specified ID are preferred. See Renderer IDs for possible values. You can pass this constant to the function AGL.

var AGL_SINGLE_RENDERER: Int32

var AGL_NO_RECOVERY: Int32

var AGL_ACCELERATED: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies renderers that are attached to a hardware accelerated graphics device. It is usually impossible to support more than one accelerated graphics device, because typically when a window spans more than one device, OpenGL uses the software renderer. You can pass this constant to the function AGL to find out whether a particular renderer is hardware accelerated.

var AGL_CLOSEST_POLICY: Int32

var AGL_ROBUST: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies that AGL should consider only those renderers that do not have any failure modes associated with a lack of video card resources. You can pass this constant to the function AGL.

var AGL_BACKING_STORE: Int32

var AGL_WINDOW: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies that the pixel format can be used to render to an onscreen window. You can pass this constant to the function AGL.

var AGL_MULTISCREEN: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies that the renderer is capable of driving multiple screens with the same rendering context. (A single window can span multiple screens.) You can pass this constant to the function AGL.

var AGL_VIRTUAL_SCREEN: Int32

The associated value is an integer that specifies the virtual screen number of the pixel format.

var AGL_COMPLIANT: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies a pixel format that is fully compliant with OpenGL. All macOS renderers are OpenGL-compliant. You can pass this constant to the function AGL.

var AGL_PBUFFER: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies that the renderer can render to a pixel buffer. You can pass this constant to the function AGL.

var AGL_REMOTE_PBUFFER: Int32

This constant is a Boolean attribute. If it is present in the attributes array, specifies that the renderer can render offline to a pixel buffer.

var AGL_RENDERER_ID: Int32

The associated value is a nonnegative integer that specifies a renderer. If present, OpenGL renderers that match the specified ID are preferred. See Renderer IDs for possible values. You can pass this constant to the function AGL.

var AGL_SINGLE_RENDERER: Int32

