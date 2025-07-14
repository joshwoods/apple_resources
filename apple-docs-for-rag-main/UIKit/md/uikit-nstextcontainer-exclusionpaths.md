

- UIKit
- NSTextContainer
-  exclusionPaths 

Instance Property

# exclusionPaths

An array of path objects that represents the regions where text doesn’t display in the text container.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var exclusionPaths: [UIBezierPath] { get set }
```

## Discussion

The default value of this property is an empty array. Depending on the platform, you can assign an array of NSBezierPath or UIBezierPath objects to exclude text from one or more regions in the text container’s bounds. When the layout manager proposes a line fragment rectangle intersecting one of the regions defined by the exclusion paths, the text container returns an adjusted line fragment rectangle excluding that region.

## See Also

### Related Documentation

func lineFragmentRect(forProposedRect: CGRect, at: Int, writingDirection: NSWritingDirection, remaining: UnsafeMutablePointer&lt;CGRect>?) -> CGRect

Returns the bounds of a line fragment rectangle inside the text container for the proposed rectangle.

### Defining the container shape

var size: CGSize

The size of the text container’s bounding rectangle.

var lineBreakMode: NSLineBreakMode

The behavior of the last line inside the text container.

var widthTracksTextView: Bool

A Boolean that controls whether the text container adjusts the width of its bounding rectangle when its text view resizes.

var heightTracksTextView: Bool

A Boolean that controls whether the text container adjusts the height of its bounding rectangle when its text view resizes.

