

- UIKit
- NSTextContainer
-  isSimpleRectangularTextContainer 

Instance Property

# isSimpleRectangularTextContainer

A Boolean that indicates whether the text container’s region is a rectangle with no holes or gaps, and whose edges are parallel to the text view’s coordinate system axes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var isSimpleRectangularTextContainer: Bool { get }
```

## Discussion

The value of this property is true when the text container’s region is a rectangle with no holes or gaps and the edges are parallel to the text view’s coordinate system axes. The default value of this property is false when the exclusionPaths property contains one or more items, when the maximumNumberOfLines property is not zero, or when you override the lineFragmentRect(forProposedRect:at:writingDirection:remaining:) method. Otherwise, the default value is true.

## See Also

### Constraining text layout

var maximumNumberOfLines: Int

The maximum number of lines that the text container can store.

var lineFragmentPadding: CGFloat

The value for the text inset within line fragment rectangles.

func lineFragmentRect(forProposedRect: CGRect, at: Int, writingDirection: NSWritingDirection, remaining: UnsafeMutablePointer&lt;CGRect>?) -> CGRect

Returns the bounds of a line fragment rectangle inside the text container for the proposed rectangle.

