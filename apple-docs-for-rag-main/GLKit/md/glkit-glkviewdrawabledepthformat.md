

- GLKit
-  GLKViewDrawableDepthFormat 

Enumeration

# GLKViewDrawableDepthFormat

The format of the depth renderbuffer.

iOS 5.0+iPadOS 5.0+tvOS 9.0+

``` source
enum GLKViewDrawableDepthFormat
```

## Topics

### Constants

case formatNone

The underlying framebuffer object has no depth buffer.

case format16

A 16-bit depth entry for each pixel.

case format24

A 24-bit depth entry for each pixel.

### Initializers

init?(rawValue: GLint)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum GLKViewDrawableColorFormat

The format of the color renderbuffer.

enum GLKViewDrawableStencilFormat

The format of the stencil renderbuffer.

enum GLKViewDrawableMultisample

The format of the multisampling buffer.

