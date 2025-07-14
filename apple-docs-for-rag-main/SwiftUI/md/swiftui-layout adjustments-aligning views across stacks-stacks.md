

- SwiftUI
- Layout adjustments
-  Aligning views across stacks 

Article

# Aligning views across stacks

Create a custom alignment and use it to align views across multiple stacks.

## Overview

As you nest stacks together, you may want specific items within those stacks to align with each other. By default, the alignment you specify for a stack applies only to that stack’s child views. To align child views that reside in the nested stacks, define a custom alignment, assign it to the enclosing view, and use the alignment guide modifier to identify specific views to align.

### Begin with the default center alignment

To illustrate aligning items across stacks, the following view shows a horizontal stack wrapping around two nested vertical stacks that have a different number of child views. The enclosing HStack doesn’t define an alignment, so it defaults to center.

```
struct ImageRow: View {
    var body: some View {
        HStack {
            VStack {
                Image("bell_peppers")
                    .resizable()
                    .scaledToFit()
                Text("Bell Peppers")
                    .font(.title)
            }
            VStack {
                Image("chili_peppers")
                    .resizable()
                    .scaledToFit()
                Text("Chili Peppers")
                    .font(.title)
                Text("Higher levels of capsicum")
                    .font(.caption)
            }
        }
    }
}
```

The image below shows the contents of a nested vertical stack aligning at the center of the stack. The child elements within the vertical stacks, such as the titles beneath each image, don’t align with each other.

### Define a custom alignment

To create a new vertical alignment guide, extend VerticalAlignment with a new static property for your guide. Name the guide according to what it aligns to make it easier to use. The following example uses bottom positioning as the default value for this guide:

```
extension VerticalAlignment {
    /// A custom alignment for image titles.
    private struct ImageTitleAlignment: AlignmentID {
        static func defaultValue(in context: ViewDimensions) -> CGFloat {
            // Default to bottom alignment if no guides are set.
            context[VerticalAlignment.bottom]
        }
    }

    /// A guide for aligning titles.
    static let imageTitleAlignmentGuide = VerticalAlignment(
        ImageTitleAlignment.self
    )
}
```

### Assign and apply the custom alignment

To use the alignment guide, assign it to a parent view that encloses the views you want to align. The following example specifies `imageTitleAlignmentGuide` as the alignment for the horizontal stack:

```
struct RowOfAlignedImages: View {
    var body: some View {
        HStack(alignment: .imageTitleAlignmentGuide) {
            VStack {
                Image("bell_peppers")
                    .resizable()
                    .scaledToFit()

                Text("Bell Peppers")
                    .font(.title)
            }
            VStack {
                Image("chili_peppers")
                    .resizable()
                    .scaledToFit()

                Text("Chili Peppers")
                    .font(.title)

                Text("Higher levels of capsicum")
                    .font(.caption)
            }
        }
    }
}
```

The two vertical stacks now align on the bottoms of the stacks, using the default from your specification for the custom guide.

When you define an alignment on a stack, it projects through enclosed child views. Within the nested VStack instances, apply alignmentGuide(_:computeValue:) to the views to align, using your custom guide for the HStack.

```
struct RowOfAlignedImages: View {
    var body: some View {
        HStack(alignment: .imageTitleAlignmentGuide) {
            VStack {
                Image("bell_peppers")
                    .resizable()
                    .scaledToFit()

                Text("Bell Peppers")
                    .font(.title)
                    .alignmentGuide(.imageTitleAlignmentGuide) { context in
                        context[.firstTextBaseline]
                    }
            }
            VStack {
                Image("chili_peppers")
                    .resizable()
                    .scaledToFit()

                Text("Chili Peppers")
                    .font(.title)
                    .alignmentGuide(.imageTitleAlignmentGuide) { context in
                        context[.firstTextBaseline]
                    }

                Text("Higher levels of capsicum")
                    .font(.caption)
            }
        }
    }
}
```

The closure from the alignment guide modifier returns firstTextBaseline, which aligns the baselines of the titles with the alignment guide `imageTitleAlignmentGuide`.

## See Also

### Aligning views

Aligning views within a stack

Position views inside a stack using alignment guides.

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

struct ViewDimensions

A view’s size and alignment guides in its own coordinate space.

