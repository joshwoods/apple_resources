

- SwiftUI
-  DepthAlignment 

Structure

# DepthAlignment

An alignment position along the depth axis.

visionOS 1.0+

``` source
@frozen
struct DepthAlignment
```

## Topics

### Getting guides

static let back: DepthAlignment

A guide marking the bottom edge of the view.

static let center: DepthAlignment

A guide marking the vertical center of the view.

static let front: DepthAlignment

A guide marking the top edge of the view.

## Relationships

### Conforms To

- Equatable

## See Also

### Aligning views

Aligning views within a stack

Position views inside a stack using alignment guides.

Aligning views across stacks

Create a custom alignment and use it to align views across multiple stacks.

func alignmentGuide(_:computeValue:)

Sets the view’s horizontal alignment.

struct Alignment

An alignment in both axes.

struct HorizontalAlignment

An alignment position along the horizontal axis.

struct VerticalAlignment

An alignment position along the vertical axis.

protocol AlignmentID

A type that you use to create custom alignment guides.

struct ViewDimensions

A view’s size and alignment guides in its own coordinate space.

