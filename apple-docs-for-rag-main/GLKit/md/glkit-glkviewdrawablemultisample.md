

- GLKit
-  GLKViewDrawableMultisample 

Enumeration

# GLKViewDrawableMultisample

The format of the multisampling buffer.

iOS 5.0+iPadOS 5.0+tvOS 9.0+

``` source
enum GLKViewDrawableMultisample
```

## Overview

Multisampling improves the quality of the output image, but may require more memory and image processing to do so. As such, you should profile your application with and without multisampling enabled, and choose a setting that provides both the image quality and performance you require.

## Topics

### Constants

case multisampleNone

Multisampling is not enabled.

case multisample4X

Multisampling is enabled.

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

enum GLKViewDrawableDepthFormat

The format of the depth renderbuffer.

enum GLKViewDrawableStencilFormat

The format of the stencil renderbuffer.

