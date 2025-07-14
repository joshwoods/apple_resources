

- SwiftUI
-  ScrollTargetBehavior 

Protocol

# ScrollTargetBehavior

A type that defines the scroll behavior of a scrollable view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol ScrollTargetBehavior
```

## Overview

A scrollable view calculates where scroll gestures should end using its deceleration rate and the state of its scroll gesture by default. A scroll behavior allows for customizing this logic.

You define a scroll behavior using the updateTarget(_:context:) method.

Using this method, you can control where someone can scroll in a scrollable view. For example, you can create a custom scroll behavior that aligns to every 10 points by doing the following:

```
struct BasicScrollTargetBehavior: ScrollTargetBehavior {
    func updateTarget(_ target: inout Target, context: TargetContext) {
        // Align to every 1/10 the size of the scroll view.
        target.rect.x.round(
            toMultipleOf: round(context.containerSize.width / 10.0))
    }
}
```

### Paging Behavior

SwiftUI offers built in scroll behaviors. One such behavior is the PagingScrollTargetBehavior which uses the geometry of the scroll view to decide where to allow scrolls to end.

In the following example, every view in the lazy stack is flexible in both directions and the scroll view will settle to container aligned boundaries.

```
ScrollView {
    LazyVStack(spacing: 0.0) {
        ForEach(items) { item in
            FullScreenItem(item)
        }
    }
}
.scrollTargetBehavior(.paging)
```

### View Aligned Behavior

SwiftUI also offers a ViewAlignedScrollTargetBehavior scroll behavior that will always settle on the geometry of individual views.

```
ScrollView(.horizontal) {
    LazyHStack(spacing: 10.0) {
        ForEach(items) { item in
            ItemView(item)
        }
    }
    .scrollTargetLayout()
}
.scrollTargetBehavior(.viewAligned)
.safeAreaPadding(.horizontal, 20.0)
```

You configure which views should be used for settling using the scrollTargetLayout(isEnabled:) modifier. Apply this modifier to a layout container like LazyVStack or HStack and each individual view in that layout will be considered for alignment.

Use types conforming to this protocol with the scrollTargetBehavior(_:) modifier.

## Topics

### Getting the scroll target behavior

static var paging: PagingScrollTargetBehavior

The scroll behavior that aligns scroll targets to container-based geometry.

static var viewAligned: ViewAlignedScrollTargetBehavior

The scroll behavior that aligns scroll targets to view-based geometry.

static func viewAligned(limitBehavior: ViewAlignedScrollTargetBehavior.LimitBehavior) -> Self

The scroll behavior that aligns scroll targets to view-based geometry.

### Updating the proposed target

func updateTarget(inout ScrollTarget, context: Self.TargetContext)

Updates the proposed target that a scrollable view should scroll to.

**Required**

typealias TargetContext

The context in which a scroll behavior updates the scroll target.

### Instance Methods

func properties(context: Self.PropertiesContext) -> Self.Properties

Properties of this behavior

**Required** Default implementation provided.

### Type Aliases

typealias Properties

The properties of a scroll behavior

typealias PropertiesContext

The properties context of a scroll behavior.

## Relationships

### Conforming Types

- AnyScrollTargetBehavior
- PagingScrollTargetBehavior
- ViewAlignedScrollTargetBehavior

## See Also

### Defining scroll targets

func scrollTargetBehavior(some ScrollTargetBehavior) -> some View

Sets the scroll behavior of views scrollable in the provided axes.

func scrollTargetLayout(isEnabled: Bool) -> some View

Configures the outermost layout as a scroll target layout.

struct ScrollTarget

A type defining the target in which a scroll view should try and scroll to.

struct ScrollTargetBehaviorContext

The context in which a scroll target behavior updates its scroll target.

struct PagingScrollTargetBehavior

The scroll behavior that aligns scroll targets to container-based geometry.

struct ViewAlignedScrollTargetBehavior

The scroll behavior that aligns scroll targets to view-based geometry.

struct AnyScrollTargetBehavior

A type-erased scroll target behavior.

