

- SwiftUI
-  ScrollAnchorRole 

Structure

# ScrollAnchorRole

A type defining the role of a scroll anchor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ScrollAnchorRole
```

## Overview

You can associate a UnitPoint to a ScrollView using the defaultScrollAnchor(_:) modifier. By default, the system uses this point for different kinds of behaviors including:

- Where the scroll view should initially be scrolled

- How the scroll view should handle content size or container size changes

- How the scroll view should align content smaller than its container size

You can further customize this behavior by assigning different unit points for these different roles.

## Topics

### Type Properties

static var alignment: ScrollAnchorRole

The role that influences how a scroll view should align its content when the size of its content is smaller than the container size of the scroll view.

static var initialOffset: ScrollAnchorRole

The role that influences where a scroll view should be initially scrolled.

static var sizeChanges: ScrollAnchorRole

The role that influences how a scroll view should adjust its content offset when the scroll view’s content or container size changes.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Managing scroll position

func scrollPosition(Binding&lt;ScrollPosition>, anchor: UnitPoint?) -> some View

Associates a binding to a scroll position with a scroll view within this view.

func scrollPosition(id: Binding&lt;(some Hashable)?>, anchor: UnitPoint?) -> some View

Associates a binding to be updated when a scroll view within this view scrolls.

func defaultScrollAnchor(UnitPoint?) -> some View

Associates an anchor to control which part of the scroll view’s content should be rendered by default.

func defaultScrollAnchor(UnitPoint?, for: ScrollAnchorRole) -> some View

Associates an anchor to control the position of a scroll view in a particular circumstance.

struct ScrollPosition

A type that defines the semantic position of where a scroll view is scrolled within its content.

