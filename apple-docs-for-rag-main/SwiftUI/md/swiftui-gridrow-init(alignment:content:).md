

- SwiftUI
- GridRow
-  init(alignment:content:) 

Initializer

# init(alignment:content:)

Creates a horizontal row of child views in a grid.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    alignment: VerticalAlignment? = nil,
    @ViewBuilder content: () -> Content
)
```

## Parameters 

`alignment`  

An optional VerticalAlignment for the row. If you don’t specify a value, the row uses the vertical alignment component of the Alignment parameter that you specify in the grid’s init(alignment:horizontalSpacing:verticalSpacing:content:) initializer, which is center by default.

`content`  

The builder closure that contains the child views. Each view in the closure implicitly maps to a cell in the grid.

## Discussion

Use this initializer to create a GridRow inside of a Grid. Provide a content closure that defines the cells of the row, and optionally customize the vertical alignment of content within each cell. The following example customizes the vertical alignment of the cells in the first and third rows:

```
Grid(alignment: .trailing) {
    GridRow(alignment: .top) { // Use top vertical alignment.
        Text("Top")
        Color.red.frame(width: 1, height: 50)
        Color.blue.frame(width: 50, height: 1)
    }
    GridRow { // Use the default (center) alignment.
        Text("Center")
        Color.red.frame(width: 1, height: 50)
        Color.blue.frame(width: 50, height: 1)
    }
    GridRow(alignment: .bottom) { // Use bottom vertical alignment.
        Text("Bottom")
        Color.red.frame(width: 1, height: 50)
        Color.blue.frame(width: 50, height: 1)
    }
}
```

The example above specifies trailing alignment for the grid, which is composed of center vertical alignment and trailing horizontal alignment. The middle row relies on the center vertical alignment, but the other two rows specify custom vertical alignments:

Important

A grid row behaves like a Group if you create it outside of a grid.

To override column alignment, use gridColumnAlignment(_:). To override alignment for a single cell, use gridCellAnchor(_:).

