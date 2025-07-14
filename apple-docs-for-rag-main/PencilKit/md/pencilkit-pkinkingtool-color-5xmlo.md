

- PencilKit
- PKInkingTool
-  color 

Instance Property

# color

The color of the ink.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
var color: UIColor { get set }
```

## Discussion

The alpha of the final color may vary due to input from Apple Pencil. For example, light pressure from Apple Pencil introduces more transparency into the final color, while additional force increases opacity to create a more solid line.

## See Also

### Getting the inking tool attributes

var color: NSColor

The color of the ink.

var width: CGFloat

The width of the ink.

var ink: PKInk

The ink used by this inking tool.

