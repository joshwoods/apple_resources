

- AppKit
- NSImage
-  NSImage.ResizingMode 

Enumeration

# NSImage.ResizingMode

Constants that describe the resizing mode for the image.

macOS 10.10+

``` source
enum ResizingMode
```

## Topics

### Constants

case tile

The image tiles when it resizes.

case stretch

The image stretches when it resizes.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Drawing Options

var isValid: Bool

A Boolean value that indicates whether it is possible to draw an image representation.

var backgroundColor: NSColor

The background color for the image.

var capInsets: NSEdgeInsets

The cap insets for the image.

var resizingMode: NSImage.ResizingMode

The resizing mode for the image.

