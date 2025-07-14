

- UIKit
- NSTextContainer
-  size 

Instance Property

# size

The size of the text container’s bounding rectangle.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var size: CGSize { get set }
```

## Discussion

This property defines the maximum size for the layout area returned from lineFragmentRect(forProposedRect:at:writingDirection:remaining:). A value of `0.0` or less means no limitation.

If you don’t specify an explicit size when you initialize a text container, the system uses a default large size of (`10000000.0`, `10000000.0`).

## See Also

### Defining the container shape

var exclusionPaths: [UIBezierPath]

An array of path objects that represents the regions where text doesn’t display in the text container.

var lineBreakMode: NSLineBreakMode

The behavior of the last line inside the text container.

var widthTracksTextView: Bool

A Boolean that controls whether the text container adjusts the width of its bounding rectangle when its text view resizes.

var heightTracksTextView: Bool

A Boolean that controls whether the text container adjusts the height of its bounding rectangle when its text view resizes.

