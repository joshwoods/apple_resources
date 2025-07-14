

- SwiftUI
-  ViewDimensions 

Structure

# ViewDimensions

A view’s size and alignment guides in its own coordinate space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ViewDimensions
```

## Mentioned in 

Aligning views within a stack

## Overview

This structure contains the size and alignment guides of a view. You receive an instance of this structure to use in a variety of layout calculations, like when you:

- Define a default value for a custom alignment guide; see defaultValue(in:).

- Modify an alignment guide on a view; see alignmentGuide(_:computeValue:).

- Ask for the dimensions of a subview of a custom view layout; see dimensions(in:).

### Custom alignment guides

You receive an instance of this structure as the `context` parameter to the defaultValue(in:) method that you implement to produce the default offset for an alignment guide, or as the first argument to the closure you provide to the alignmentGuide(_:computeValue:) view modifier to override the default calculation for an alignment guide. In both cases you can use the instance, if helpful, to calculate the offset for the guide. For example, you could compute a default offset for a custom VerticalAlignment as a fraction of the view’s height:

```
private struct FirstThirdAlignment: AlignmentID {
    static func defaultValue(in context: ViewDimensions) -> CGFloat {
        context.height / 3
    }
}

extension VerticalAlignment {
    static let firstThird = VerticalAlignment(FirstThirdAlignment.self)
}
```

As another example, you could use the view dimensions instance to look up the offset of an existing guide and modify it:

```
struct ViewDimensionsOffset: View {
    var body: some View {
        VStack(alignment: .leading) {
            Text("Default")
            Text("Indented")
                .alignmentGuide(.leading) { context in
                    context[.leading] - 10
                }
        }
    }
}
```

The example above indents the second text view because the subtraction moves the second text view’s leading guide in the negative x direction, which is to the left in the view’s coordinate space. As a result, SwiftUI moves the second text view to the right, relative to the first text view, to keep their leading guides aligned:

### Layout direction

The discussion above describes a left-to-right language environment, but you don’t change your guide calculation to operate in a right-to-left environment. SwiftUI moves the view’s origin from the left to the right side of the view and inverts the positive x direction. As a result, the existing calculation produces the same effect, but in the opposite direction.

You can see this if you use the environment(_:_:) modifier to set the layoutDirection property for the view that you defined above:

```
ViewDimensionsOffset()
    .environment(\.layoutDirection, .rightToLeft)
```

With no change in your guide, this produces the desired effect — it indents the second text view’s right side, relative to the first text view’s right side. The leading edge is now on the right, and the direction of the offset is reversed:

## Topics

### Getting dimensions

var height: CGFloat

The view’s height.

var width: CGFloat

The view’s width.

### Accessing guide values

subscript(_:)

Gets the value of the given horizontal guide.

subscript(explicit:)

Gets the explicit value of the given horizontal alignment guide.

## Relationships

### Conforms To

- Copyable
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

struct DepthAlignment

An alignment position along the depth axis.

protocol AlignmentID

A type that you use to create custom alignment guides.

