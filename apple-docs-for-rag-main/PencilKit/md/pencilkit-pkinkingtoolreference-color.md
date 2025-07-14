

- PencilKit
- PKInkingToolReference
-  color 

Instance Property

# color

The color of the ink.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
var color: UIColor { get }
```

**macOS**

``` source
var color: NSColor { get }
```

## Discussion

The alpha of the final color may vary due to input from Apple Pencil. For example, light pressure from Apple Pencil introduces more transparency into the final color, while additional force increases opacity to create a more solid line.

## See Also

### Getting the inking tool attributes

var width: CGFloat

The base line width for new content.

var ink: PKInk

The ink that this tool creates strokes with.

