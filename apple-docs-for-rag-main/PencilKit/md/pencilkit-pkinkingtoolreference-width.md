

- PencilKit
- PKInkingToolReference
-  width 

Instance Property

# width

The base line width for new content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var width: CGFloat { get }
```

## Discussion

The actual line width at any given point varies based on input from Apple Pencil. For finger-based drawing, the line width is equal to the value in this property.

## See Also

### Getting the inking tool attributes

var color: UIColor

The color of the ink.

var ink: PKInk

The ink that this tool creates strokes with.

