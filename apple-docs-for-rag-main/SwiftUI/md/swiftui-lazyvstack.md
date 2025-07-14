

- SwiftUI
-  LazyVStack 

Structure

# LazyVStack

A view that arranges its children in a line that grows vertically, creating items only as needed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct LazyVStack where Content : View
```

## Mentioned in 

Picking container views for your content

Grouping data with lazy stack views

Displaying data in lists

Creating performant scrollable stacks

## Overview

The stack is “lazy,” in that the stack view doesn’t create items until it needs to render them onscreen.

In the following example, a ScrollView contains a `LazyVStack` that consists of a vertical row of text views. The stack aligns to the leading edge of the scroll view, and uses default spacing between the text views.

```
ScrollView {
    LazyVStack(alignment: .leading) {
        ForEach(1...100, id: \.self) {
            Text("Row \($0)")
        }
    }
}
```

## Topics

### Creating a lazy-loading vertical stack

init(alignment: HorizontalAlignment, spacing: CGFloat?, pinnedViews: PinnedScrollableViews, content: () -> Content)

Creates a lazy vertical stack view with the given spacing, vertical alignment, pinning behavior, and content.

## Relationships

### Conforms To

- View

## See Also

### Dynamically arranging views in one dimension

Grouping data with lazy stack views

Split content into logical sections inside lazy stack views.

Creating performant scrollable stacks

Display large numbers of repeated views efficiently with scroll views, stack views, and lazy stacks.

struct LazyHStack

A view that arranges its children in a line that grows horizontally, creating items only as needed.

struct PinnedScrollableViews

A set of view types that may be pinned to the bounds of a scroll view.

