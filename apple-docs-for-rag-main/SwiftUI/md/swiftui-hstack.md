

- SwiftUI
-  HStack 

Structure

# HStack

A view that arranges its subviews in a horizontal line.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct HStack where Content : View
```

## Mentioned in 

Building layouts with stack views

Creating performant scrollable stacks

Laying out a simple view

Picking container views for your content

Aligning views within a stack

## Overview

Unlike LazyHStack, which only renders the views when your app needs to display them onscreen, an `HStack` renders the views all at once, regardless of whether they are on- or offscreen. Use the regular `HStack` when you have a small number of subviews or don’t want the delayed rendering behavior of the “lazy” version.

The following example shows a simple horizontal stack of five text views:

```
var body: some View {
    HStack(
        alignment: .top,
        spacing: 10
    ) {
        ForEach(
            1...5,
            id: \.self
        ) {
            Text("Item \($0)")
        }
    }
}
```

Note

If you need a horizontal stack that conforms to the Layout protocol, like when you want to create a conditional layout using AnyLayout, use HStackLayout instead.

## Topics

### Creating a stack

init(alignment: VerticalAlignment, spacing: CGFloat?, content: () -> Content)

Creates a horizontal stack with the given spacing and vertical alignment.

## Relationships

### Conforms To

- View

## See Also

### Statically arranging views in one dimension

Building layouts with stack views

Compose complex layouts from primitive container views.

struct VStack

A view that arranges its subviews in a vertical line.

