

- AppKit
- NSView
-  isDrawingFindIndicator 

Instance Property

# isDrawingFindIndicator

A Boolean value indicating whether the view or one of its ancestors is being drawn for a find indicator.

macOS 10.7+

``` source
@MainActor
var isDrawingFindIndicator: Bool { get }
```

## Discussion

The value of this property is true when the view contents are being drawn so that they are easily readable against the find indicator background. The default value of this property is false.

