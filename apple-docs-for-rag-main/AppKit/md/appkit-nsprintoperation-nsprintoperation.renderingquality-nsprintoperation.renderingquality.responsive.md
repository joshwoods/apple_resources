

- AppKit
- NSPrintOperation
- NSPrintOperation.RenderingQuality
-  NSPrintOperation.RenderingQuality.responsive 

Case

# NSPrintOperation.RenderingQuality.responsive

Sacrifices the least possible amount of rendering quality for speed to maintain a responsive user interface. This option should be used only after establishing that best quality rendering does indeed make the user interface unresponsive.

macOS 10.7+

``` source
case responsive
```

## See Also

### Constants

case best

Renders the printing at the best possible quality, regardless of speed.

