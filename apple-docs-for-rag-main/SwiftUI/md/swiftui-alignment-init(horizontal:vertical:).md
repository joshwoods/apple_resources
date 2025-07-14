

- SwiftUI
- Alignment
-  init(horizontal:vertical:) 

Initializer

# init(horizontal:vertical:)

Creates a custom alignment value with the specified horizontal and vertical alignment guides.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    horizontal: HorizontalAlignment,
    vertical: VerticalAlignment
)
```

## Parameters 

`horizontal`  

The alignment on the horizontal axis.

`vertical`  

The alignment on the vertical axis.

## Discussion

SwiftUI provides a variety of built-in alignments that combine built-in HorizontalAlignment and VerticalAlignment guides. Use this initializer to create a custom alignment that makes use of a custom horizontal or vertical guide, or both.

For example, you can combine a custom vertical guide called `firstThird` with the built-in center guide, and use it to configure a ZStack:

```
ZStack(alignment: Alignment(horizontal: .center, vertical: .firstThird)) {
    // ...
}
```

For more information about creating custom guides, including the code that creates the custom `firstThird` alignment in the example above, see AlignmentID.

## See Also

### Creating a custom alignment

var horizontal: HorizontalAlignment

The alignment on the horizontal axis.

var vertical: VerticalAlignment

The alignment on the vertical axis.

