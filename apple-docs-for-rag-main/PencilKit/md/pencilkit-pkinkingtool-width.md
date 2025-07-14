

- PencilKit
- PKInkingTool
-  width 

Instance Property

# width

The width of the ink.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
var width: CGFloat { get set }
```

## Discussion

The actual line width at any given point varies based on input from Apple Pencil. For finger-based drawing, the line width is equal to the value in this property.

## See Also

### Getting the inking tool attributes

var color: UIColor

The color of the ink.

var color: NSColor

The color of the ink.

var ink: PKInk

The ink used by this inking tool.

