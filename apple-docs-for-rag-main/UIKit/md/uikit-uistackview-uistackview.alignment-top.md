

- UIKit
- UIStackView
- UIStackView.Alignment
-  top 

Type Property

# top

A layout for horizontal stacks where the stack view aligns the top edge of its arranged views along its top edge.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
static var top: UIStackView.Alignment { get }
```

## Discussion

This value is equivalent to the UIStackView.Alignment.leading alignment for vertical stacks.

The following image shows an example of a horizontal stack view that uses the top alignment.

## See Also

### Constants

case fill

A layout where the stack view resizes its arranged views so that they fill the available space perpendicular to the stack view’s axis.

case center

A layout where the stack view aligns the center of its arranged views with its center along its axis.

case leading

A layout for vertical stacks where the stack view aligns the leading edge of its arranged views along its leading edge.

case trailing

A layout for vertical stacks where the stack view aligns the trailing edge of its arranged views along its trailing edge.

static var bottom: UIStackView.Alignment

A layout for horizontal stacks where the stack view aligns the bottom edge of its arranged views along its bottom edge.

case firstBaseline

A layout for horizontal stacks where the stack view aligns its arranged views based on their first baseline.

case lastBaseline

A layout for horizontal stacks where the stack view aligns its arranged views based on their last baseline.

