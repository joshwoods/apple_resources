

- SwiftUI
- View
-  alignmentGuide(\_:computeValue:) 

Instance Method

# alignmentGuide(\_:computeValue:)

Sets the view’s horizontal alignment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency nonisolated
func alignmentGuide(
    _ g: HorizontalAlignment,
    computeValue: @escaping (ViewDimensions) -> CGFloat
) -> some View
```

Show all declarations

## Parameters 

`g`  

A HorizontalAlignment value at which to base the offset.

`computeValue`  

A closure that returns the offset value to apply to this view.

## Return Value

A view modified with respect to its horizontal alignment according to the computation performed in the method’s closure.

## Mentioned in 

Aligning views within a stack

Aligning views across stacks

## Discussion

Use `alignmentGuide(_:computeValue:)` to calculate specific offsets to reposition views in relationship to one another. You can return a constant or can use the ViewDimensions argument to the closure to calculate a return value.

In the example below, the HStack is offset by a constant of 50 points to the right of center:

```
VStack {
    Text("Today's Weather")
        .font(.title)
        .border(.gray)
    HStack {
        Text("🌧")
        Text("Rain & Thunderstorms")
        Text("⛈")
    }
    .alignmentGuide(HorizontalAlignment.center) { _ in  50 }
    .border(.gray)
}
.border(.gray)
```

Changing the alignment of one view may have effects on surrounding views. Here the offset values inside a stack and its contained views is the difference of their absolute offsets.

## See Also

### Aligning views

Aligning views within a stack

Position views inside a stack using alignment guides.

Aligning views across stacks

Create a custom alignment and use it to align views across multiple stacks.

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

struct ViewDimensions

A view’s size and alignment guides in its own coordinate space.

