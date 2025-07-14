

- AppKit
- NSTextContainer
-  widthTracksTextView 

Instance Property

# widthTracksTextView

A Boolean that controls whether the text container adjusts the width of its bounding rectangle when its text view resizes.

macOS 10.0+

``` source
var widthTracksTextView: Bool { get set }
```

## Discussion

When the value of this property is true, the text container adjusts its width when the width of its text view changes. The default value of this property is false.

For more information about size tracking, see Text System Storage Layer Overview.

## See Also

### Defining the container shape

var size: CGSize

The size of the text container’s bounding rectangle.

var exclusionPaths: [NSBezierPath]

An array of path objects that represents the regions where text doesn’t display in the text container.

var lineBreakMode: NSLineBreakMode

The behavior of the last line inside the text container.

var heightTracksTextView: Bool

A Boolean that controls whether the text container adjusts the height of its bounding rectangle when its text view resizes.

