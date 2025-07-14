

- AppKit
- NSTextContainer
-  lineBreakMode 

Instance Property

# lineBreakMode

The behavior of the last line inside the text container.

macOS 10.11+

``` source
var lineBreakMode: NSLineBreakMode { get set }
```

## Discussion

The NSLineBreakMode constants specify what happens when a line is too long for its container. For example, wrapping can occur on word boundaries (the default) or character boundaries, or the line can be clipped or truncated. The default value of this property is NSLineBreakMode.byWordWrapping.

## See Also

### Defining the container shape

var size: CGSize

The size of the text container’s bounding rectangle.

var exclusionPaths: [NSBezierPath]

An array of path objects that represents the regions where text doesn’t display in the text container.

var widthTracksTextView: Bool

A Boolean that controls whether the text container adjusts the width of its bounding rectangle when its text view resizes.

var heightTracksTextView: Bool

A Boolean that controls whether the text container adjusts the height of its bounding rectangle when its text view resizes.

