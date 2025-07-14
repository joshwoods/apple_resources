

- SwiftUI
- Alignment
-  horizontal 

Instance Property

# horizontal

The alignment on the horizontal axis.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var horizontal: HorizontalAlignment
```

## Discussion

Set this value when you initialize an alignment using the init(horizontal:vertical:) method. Use one of the built-in HorizontalAlignment guides, like center, or a custom guide that you create.

For information about creating custom guides, see AlignmentID.

## See Also

### Creating a custom alignment

init(horizontal: HorizontalAlignment, vertical: VerticalAlignment)

Creates a custom alignment value with the specified horizontal and vertical alignment guides.

var vertical: VerticalAlignment

The alignment on the vertical axis.

