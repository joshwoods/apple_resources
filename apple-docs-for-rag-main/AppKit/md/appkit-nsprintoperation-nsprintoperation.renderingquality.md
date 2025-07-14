

- AppKit
- NSPrintOperation
-  NSPrintOperation.RenderingQuality 

Enumeration

# NSPrintOperation.RenderingQuality

Constants that specify the print quality in use.

macOS 10.7+

``` source
enum RenderingQuality
```

## Topics

### Constants

case best

Renders the printing at the best possible quality, regardless of speed.

case responsive

Sacrifices the least possible amount of rendering quality for speed to maintain a responsive user interface. This option should be used only after establishing that best quality rendering does indeed make the user interface unresponsive.

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

### Getting the Printing Quality

var preferredRenderingQuality: NSPrintOperation.RenderingQuality

The printing quality.

