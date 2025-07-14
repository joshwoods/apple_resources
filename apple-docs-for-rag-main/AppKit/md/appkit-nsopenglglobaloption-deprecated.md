

- AppKit
-  NSOpenGLGlobalOption Deprecated

Enumeration

# NSOpenGLGlobalOption

Constants that specify OpenGL options.

macOS 10.0–10.14Deprecated

``` source
enum NSOpenGLGlobalOption
```

Deprecated

The OpenGL API is deprecated. Use Metal and MetalKit instead.

## Overview

These constants are option names for NSOpenGLSetOption and NSOpenGLGetOption.

## Topics

### Constants

case formatCacheSize

Sets the size of the pixel format cache.

case clearFormatCache

Resets the pixel format cache if true.

case retainRenderers

Whether to retain loaded renderers in memory.

case useBuildCache

Whether to enable the function compilation block cache. This is off by default. It must be enabled at startup.

### Deprecated

var globalValue: GLint

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum NSMultibyteGlyphPacking

A constant for glyph packing.

Deprecated

Glyph Attributes

Attributes that are used only inside the glyph generation machinery, but must also be shared between components.

Data Entry Types

These constants specify how a cell formats numeric data.

Anonymous

Additional Writing Directions

Additional values to be added to NSWritingDirection.leftToRight or NSWritingDirection.rightToLeft, when used with writingDirection.

Return values for modal operations

Historical return values for runModal(for:) and runModalSession(_:).

Tags of Views in the FontPanel

These constants are obsolete and should not be used.

